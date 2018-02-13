FROM docker.elastic.co/beats/filebeat:6.2.1

MAINTAINER indrajit<eendroroy@gmail.com>

COPY filebeat.yml /usr/share/filebeat/filebeat.yml

USER root

RUN chown filebeat /usr/share/filebeat/filebeat.yml

USER filebeat

RUN filebeat modules enable nginx
