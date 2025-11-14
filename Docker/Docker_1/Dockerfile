FROM ubuntu
ENV TZ=Asia/Kolkata
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone
RUN apt-get update
RUN apt-get -y install apache2
ADD ./2145_eco_lume /var/www/html
ENTRYPOINT apachectl -D FOREGROUND
ENV name Devopstesting
