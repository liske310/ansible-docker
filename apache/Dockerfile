FROM ubuntu:latest
MAINTAINER liske1 <liske310@protonmail.com>
# Install apache
RUN apt-get update && apt-get install -y apache2

# Export VARIABLES for run apache
ENV "APACHE_PID_FILE"="/var/run/apache2.pid"
ENV "APACHE_LOG_DIR"="/var/log"
ENV "APACHE_RUN_GROUP"="www-data"
ENV "APACHE_RUN_USER"="www-data"
ENV "APACHE_RUN_DIR"="/var/run"

# Run apache in foreground
ENTRYPOINT ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"]
