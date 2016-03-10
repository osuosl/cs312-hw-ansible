FROM nginx
MAINTAINER cs312@osuosl.org

RUN apt-get update
RUN apt-get install -y build-essential python-dev python-virtualenv git libjpeg-dev zlib1g-dev

RUN git clone https://github.com/osuosl/cs312
WORKDIR /cs312
RUN bash scripts/build.sh
RUN cp -r build/html/* /usr/share/nginx/html
