FROM nginx:1.23.4-alpine as nginx

ARG VERSION

LABEL org.opencontainers.image.version="$VERSION"
LABEL org.opencontainers.image.authors="Wojciech Dziedzic"

COPY nginx.conf /etc/nginx/conf.d/default.conf 
COPY index.php /usr/share/nginx/html/index.php

EXPOSE 6002

CMD ["nginx", "-g", "daemon off;"]