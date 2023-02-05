FROM ubuntu:22.04
RUN apt update -y
RUN apt upgrade -y
RUN apt install wget -y
RUN apt install iputils-ping -y
RUN apt-get --quiet update \
&& apt-get --quiet --yes upgrade \
&& apt-get --quiet --yes install ca-certificates-java git curl unzip wget apt-utils tar unzip build-essential \
&& apt-get --quiet --yes install vim-common \
&& apt-get --quiet update && apt-get --quiet --yes install openjdk-17-jdk openjdk-17-jre
COPY . /app
WORKDIR /app
ENTRYPOINT ["./cmd.sh"]
