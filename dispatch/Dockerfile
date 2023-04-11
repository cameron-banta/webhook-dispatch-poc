FROM openresty/openresty:bullseye
# RUN apk add lua5.1-cjson
RUN apt-get update && apt-get install lua-cjson
COPY conf.d /etc/nginx/conf.d
COPY nginx.conf /etc/nginx/
COPY env.conf /etc/nginx/
