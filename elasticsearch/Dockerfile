FROM docker.elastic.co/elasticsearch/elasticsearch-oss:7.5.0

EXPOSE 9200 9300

COPY ./synonyms.txt /usr/share/elasticsearch/config/analysis/synonyms.txt

RUN /usr/share/elasticsearch/bin/elasticsearch-plugin install analysis-phonetic
