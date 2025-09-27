FROM ubuntu:24.04
WORKDIR /files
RUN apt update
RUN apt install nginx -y
RUN apt install wget -y
RUN apt install unzip -y
RUN wget https://templatemo.com/tm-zip-files-2020/templatemo_556_catalog_z.zip
RUN unzip templatemo_556_catalog_z.zip
RUN cp -r templatemo_556_catalog_z  /var/www/html
EXPOSE 80
CMD ["nginx","start","--host","0.0.0.0"]