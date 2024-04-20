FROM nginx
#WORKDIR /task
#COPY . /task
RUN rm /etc/nginx/nginx.conf
RUN mkdir /etc/nginx/ssl/
COPY default /etc/nginx/sites-enabled/default
COPY nginx.conf /etc/nginx/nginx.conf
COPY ./ssl/nginx.crt /etc/nginx/ssl/
COPY ./ssl/nginx.key /etc/nginx/ssl/
COPY hosts /etc/hosts
COPY proxy_params /etc/nginx/proxy_params
#CMD ["nginx", "-g", "daemon off;"]
CMD nginx
#EXPOSE 5000
