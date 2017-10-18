# Docker image - example
FROM ubuntu:14.04
# init.
RUN apt-get update
RUN apt-get install -y build-essential && apt-get -y dist-upgrade && apt-get -y upgrade
RUN apt-get install -y libsvm-tools default-jre default-jdk rsync vim curl wget 
RUN cp /usr/share/zoneinfo/Asia/Taipei /etc/localtime
#### run container
EXPOSE 22
CMD ["/usr/sbin/sshd", "-D"]
# tools - nodejs & npm & ls
RUN wget https://nodejs.org/dist/v4.2.1/node-v4.2.1.tar.gz
RUN tar zxvf node-v4.2.1.tar.gz && cd node-v4.2.1 && ./configure && make && make install
RUN npm update -g npm
RUN npm install -g livescript
