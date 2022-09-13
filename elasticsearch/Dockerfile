#ddev-generated
FROM elasticsearch:7.17.6
# if there is an elasticsearch.yml in elasticsearch directory
# it will get copied into elasticsearch config.
#COPY /elasticsearch/* /usr/share/elasticsearch/config/
WORKDIR /usr/share/elasticsearch

ENV cluster.name=docker-cluster
ENV bootstrap.memory_lock=true
ENV ES_JAVA_OPTS="-Xms1024m -Xmx1024m"

RUN bin/elasticsearch-plugin install analysis-phonetic
RUN bin/elasticsearch-plugin install analysis-icu
