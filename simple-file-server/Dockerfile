FROM nginx:1.11.13

MAINTAINER jiwei <jiwei@nonexist.top>
RUN echo '\
server {\n\
        listen       80;\n\
        server_name  ftp.server;\n\
        client_max_body_size 2048M;\n\
        root  /data;\n\
        autoindex on;\n\
        autoindex_exact_size off;\n\
        autoindex_localtime on;\n\
        default_type  application/octet-stream;\n\
        location / {\n\
        }\n\
}' > /etc/nginx/conf.d/default.conf
VOLUME /data
