# Use the httpd-parent image as base
FROM quay.io/redhattraining/httpd-parent
EXPOSE 8080
RUN sed -i 's/^Listen 80/&80/' /etc/httpd/conf/httpd.conf && \
    chgrp -R 0 /var/log/httpd /var/run/httpd && \
    chmod -R 770 /var/log/httpd /var/run/httpd
USER 1001
