FROM httpd:2.4-alpine

COPY ./httpd.conf /usr/local/apache2/conf/drupal.conf

RUN echo "Include /usr/local/apache2/conf/drupal.conf" \
    >> /usr/local/apache2/conf/httpd.conf

RUN sed -i '/LoadModule rewrite_module/s/^#//g' /usr/local/apache2/conf/drupal.conf