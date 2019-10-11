# Use the httpd-parent image as base
FROM quay.io/redhattraining/httpd-parent
EXPOSE 8080
LABEL io.k8s.description="A basic Apache HTTP Server child image, uses ONBUILD" \
      io.openshift.expose-servies="8080:http" \
      io.k8s.display-name="Apache HTTP Server" \
      io.openshift.tags="apache, httpd"
RUN sed -i "s/Lisen 80/Listen 8080/g" /etc/httpd/conf/httpd.conf
USER 1001
