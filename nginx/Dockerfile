FROM openresty/openresty

RUN DEBIAN_FRONTEND=noninteractive apt-get update \
    && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends \
        openresty-opm
RUN opm get 3scale/lua-resty-env
RUN echo "env APP_URL;" >> /etc/openresty/nginx.conf
COPY default.conf /etc/nginx/conf.d/default.conf

