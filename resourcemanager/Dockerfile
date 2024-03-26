FROM zhongruizhi/hadoop-base:3.3.6-java8-aarch64

LABEL org.opencontainers.image.authors="ruizhi.zhong@outlook.com"

HEALTHCHECK CMD curl -f http://localhost:8088/ || exit 1

ADD run.sh /run.sh
RUN chmod a+x /run.sh

EXPOSE 8088

CMD ["/run.sh"]
