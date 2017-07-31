FROM nginx:1.13.3-alpine

MAINTAINER arkki@arkki.tech

COPY ./nginx/conf/wordpress.conf /etc/nginx/conf.d/wordpress.conf
RUN rm /etc/nginx/conf.d/default.conf

EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]

