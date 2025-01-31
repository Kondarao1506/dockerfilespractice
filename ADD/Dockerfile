FROM almalinux:9
RUN dnf install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html
ADD https://matrix.squiz.net/manuals/asset-listing  /usr/share/nginx/html/index.html
RUN chmod 777 /usr/share/nginx/html/index.html
CMD ["nginx","-g","daemon off;"]