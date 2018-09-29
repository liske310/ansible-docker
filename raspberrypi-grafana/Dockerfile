# Pull debian ISO for armhf (raspberry PI)
FROM resin/rpi-raspbian
# If you run this not on raspberry please comment line above, and uncomment line above:
# FROM debian:latest

MAINTAINER liske1 <liske310@protonmail.com>

# Upgrade system
RUN apt-get update && apt-get upgrade

## Add repository for InfluxDB and grafana

# Install InfluxDB
RUN apt-get install InfluxDB

# Install Grafana


# Clean unnecessary archive
RUN apt-get clean

# RUN GRAFANA
