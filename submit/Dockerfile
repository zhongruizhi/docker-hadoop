FROM zhongruizhi/hadoop-base:3.3.6-java8-aarch64

LABEL org.opencontainers.image.authors="ruizhi.zhong@outlook.com"

COPY WordCount.jar /opt/hadoop/applications/WordCount.jar

ENV JAR_FILEPATH="/opt/hadoop/applications/WordCount.jar"
ENV CLASS_TO_RUN="WordCount"
ENV PARAMS="/input /output"

ADD run.sh /run.sh
RUN chmod a+x /run.sh

CMD ["/run.sh"]
