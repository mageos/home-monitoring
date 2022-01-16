FROM docker.elastic.co/logstash/logstash:7.16.3

RUN rm -f /usr/share/logstash/pipeline/logstash.conf && \
  bin/logstash-plugin install logstash-output-syslog

COPY syslog.conf /usr/share/logstash/pipeline/