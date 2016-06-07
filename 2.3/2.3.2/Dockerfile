FROM elasticsearch:2.3.2

RUN plugin install mapper-attachments
RUN plugin install analysis-phonetic
RUN plugin install license
RUN plugin install marvel-agent

RUN mkdir -p /artefacts/es
RUN chmod 777 /artefacts

RUN mkdir -p /usr/share/elasticsearch/snapshots
RUN chmod 777 /usr/share/elasticsearch/snapshots

COPY config /usr/share/elasticsearch/config
