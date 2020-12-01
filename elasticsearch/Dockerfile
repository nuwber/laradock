ARG ELK_VERSION
FROM docker.elastic.co/elasticsearch/elasticsearch:${ELK_VERSION}

EXPOSE 9200 9300

COPY ./synonyms.txt /usr/share/elasticsearch/config/analysis/synonyms.txt

RUN /usr/share/elasticsearch/bin/elasticsearch-plugin install analysis-phonetic
