#install os
FROM ubuntu

#update index and install apache2 (webserver)
RUN apt-get update \
   && apt-get install -y apache2

#copy index.html in apache2(webserver)
COPY testfile.html /var/www/html/

#virtual directory which need to expose
WORKDIR /var/www/html

#start apache2 services
CMD ["apachectl","-D","FOREGROUND"]

#export the port
EXPOSE 80
