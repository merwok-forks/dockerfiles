FROM ruby:1.9.3
MAINTAINER Jessica Frazelle <jess@docker.com>

RUN apt-get update && apt-get install -y \
	libcurl3-dev \
	--no-install-recommends \ 
	&& rm -rf /var/lib/apt/lists/* \
	&& gem install cloudapp

ENTRYPOINT ["cloudapp"]
