FROM nginx:1.23.4-alpine as nginx

ARG VERSION

LABEL org.opencontainers.image.version="$VERSION"
LABEL org.opencontainers.image.authors="Wojciech Dziedzic"

COPY nginx.conf /etc/nginx/conf.d/default.conf 