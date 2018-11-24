FROM busybox:1.29.3

LABEL maintainer="gaozhiqiang <gaozhiqiang@solomonlinux.com>"

ENV DOC_ROOT=/data/web/html

RUN \
	mkdir -p ${DOC_ROOT} \
	&& echo "Test page: Busybox:1.29.3-httpd" > ${DOC_ROOT}/index.html

EXPOSE 80/tcp
CMD /bin/httpd -f -p 80 -h ${DOC_ROOT}
