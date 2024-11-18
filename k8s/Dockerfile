FROM centos:7
Run yum update -y && yum install httpd httpd-tools -y
RUN echo "Dockerfile Test on Aapche httpd" > /var/www/html/index.html

EXPOSE 80
#CMD ["-D", "FOREGROUND"]
#ENTRYPOINT ["/usr/sbin/httpd"]
EXPOSE 80
STOPSIGNAL SIGQUIT
CMD ["/usr/sbin/httpd", "-D", "FOREGROUND"]
