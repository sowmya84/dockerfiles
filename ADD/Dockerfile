FROM almalinux:9
RUN dnf install nginx -y
RUN rm -rf /user/share/nginx/html/index.html
ADD https://github.com/DAWS-82S/dockerfiles/blob/main/RUN/Dockerfile usr/share/nginx/html/index.html
RUN chmod +r /usr/share/html/index.html
ADD samplle-1.tar /tmp/
CMD ["nginx", "-g", "daemon off;"]