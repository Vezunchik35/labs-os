FROM debian
ADD debian.list /etc/apt/sources.list.d/
RUN apt-get update && apt-get -y upgrade && apt -y install nginx && apt-get clean && \
    cd /var/www/ && rm -rf ./* && \
    mkdir -p DanilaRogozin.com/img && \
    chmod -R 754 /var/www/DanilaRogozin.com/ && \
    useradd Danila && groupadd Rogozin && usermod -aG Rogozin Danila && \
    chown -R Daniil:Semin /var/www/DanilaRogozin.com/ && \
    sed -i 's/\/var\/www\/html/\/var\/www\/DanilaRogozin/g' /etc/nginx/sites-enabled/default && \
    sed -i 's/user www-data/user Daniil/g' /etc/nginx/nginx.conf
ADD index.html /var/www/DanilaRogozin.com/
ADD img.jpg /var/www/DanilaRogozin.com/img/
CMD ["nginx", "-g", "daemon off;"]
