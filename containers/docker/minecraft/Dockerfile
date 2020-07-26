#Dockerfile v1.2
#
#
#----------------------
# CAMBIOS
# docker run -it -p 25565:25565 -v /home/minecraft:/minecraft --name 
FROM ubuntu:16.04
LABEL Augusto Morales “augusto@augustomorales.com”
LABEL Kyle Brown “brownkyl@us.ibm.com”
RUN apt-get update
RUN apt-get install default-jdk --yes
RUN apt-get install wget --yes
RUN mkdir minecraft
VOLUME /minecraft
WORKDIR /minecraft
RUN echo "eula=true" > eula.txt
RUN echo "online-mode=false" > server.properties
CMD java  -Xms512m -Xmx1024m -jar minecraft_server.jar nogui
EXPOSE 25565