#Dockerfile
FROM httpd:alpine
# Utilise image officiel

RUN apk update \
&& apk upgrade

EXPOSE 80 443
# Exposer les ports 80 et 443

WORKDIR /usr/local/apache2/
# Change dans le repertoire de configuration

COPY ./conf/httpd.conf /conf/httpd.conf
# Remplacer httpd.conf par le mien
