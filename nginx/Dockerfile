FROM openresty/openresty

RUN opm get 3scale/lua-resty-env
RUN echo "env APP_URL;" >> /etc/openresty/nginx.conf
COPY default.conf /etc/nginx/conf.d/default.conf
