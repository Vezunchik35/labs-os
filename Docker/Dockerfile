FROM debian
ADD debian.list /etc/apt/sources.list.d/
RUN apt-get update && apt-get -y upgrade && apt -y install nginx && apt-get clean && \
    cd /var/www/ && rm -rf ./* && \
    mkdir -p DalerMakhsudov.com/img && \
    chmod -R 754 /var/www/DalerMakhsudov.com/ && \
    useradd Daler && groupadd Makhsudov && usermod -aG Makhsudov Daler && \
    chown -R Daler:Makhsudov /var/www/DalerMakhsidov.com/ && \
    sed -i 's/\/var\/www\/html/\/var\/www\/DalerMakhsudov/g' /etc/nginx/sites-enabled/default && \
    sed -i 's/user www-data/user Daler/g' /etc/nginx/nginx.conf
ADD index.html /var/www/DalerMakhsudov.com/
ADD img.jpg /var/www/DalerMakhsudov.com/img/
CMD ["nginx", "-g", "daemon off;"]
