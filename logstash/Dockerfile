ARG ELKSTACK_VERSION
FROM docker.elastic.co/logstash/logstash:${ELKSTACK_VERSION}

RUN rm -f /usr/share/logstash/pipeline/logstash.conf && \
  bin/logstash-plugin install logstash-output-syslog logstash-filter-clone

COPY syslog.conf /usr/share/logstash/pipeline/