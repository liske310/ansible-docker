# ADD PORT 3000
# Pull debian ISO for armhf (raspberry PI)
FROM resin/rpi-raspbian
# If you run this not on raspberry please comment line above, and uncomment line above:
# FROM debian:latest

MAINTAINER liske1 <liske310@protonmail.com>

# Upgrade system
RUN apt-get update && apt-get upgrade
# install: apt-transport-https
RUN apt install apt-transport-https
## Add repository for InfluxDB and grafana
# curl -sL https://repos.influxdata.com/influxdb.key | apt-key add -
# test $VERSION_ID="7" && echo "deb https://repos.influxdata.com/debian wheezy stable" | sudo tee /etc/apt/sources.list.d/influxdb.list
# test $VERSION_ID="8" && echo "deb https://repos.influxdata.com/debian jessie stable" | sudo tee /etc/apt/sources.list.d/influxdb.list
# sudo apt-get update && sudo apt-get install influxdb
# INFLUXDB_CONFIG_PATH=/etc/influxdb/influxdb.conf
# Install InfluxDB
RUN apt-get install InfluxDB

# Install Grafana
#curl https://bintray.com/user/downloadSubjectPublicKey?username=bintray | sudo apt-key add -
#echo "deb https://dl.bintray.com/fg2it/deb-rpi-1b jessie main" | sudo tee -a /etc/apt/sources.list.d/grafana.list
#sudo apt-get update
#sudo apt-get install grafana


# Clean unnecessary archive
RUN apt-get clean

# RUN GRAFANA
