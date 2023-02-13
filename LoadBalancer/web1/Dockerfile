#Dockerfile
FROM httpd:alpine
# Utilise image officiel

RUN apk update \
&& apk upgrade
# Install vim et iproute pour ss

RUN mkdir /srv/htdocs
# Ajouter le repertoire pour les documents HTML

EXPOSE 80 443
# Exposer les ports 80 et 443

WORKDIR /usr/local/apache2/conf
# Change dans le repertoire de configuration

COPY ./conf/httpd.conf httpd.conf
# Remplacer httpd.conf par le mien

