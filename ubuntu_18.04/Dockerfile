FROM crops/poky:ubuntu-18.04
USER root

# Configure to prevent apt-get from getting stuck
# https://github.com/moby/moby/issues/4032#issuecomment-192327844
ARG DEBIAN_FRONTEND=noninteractive

RUN apt-get update \
	&& apt-get install -y ca-certificates \
	&& apt-get clean \
	&& rm -rf /var/lib/apt/lists/* \
	&& rm -rf /src/*.deb

USER usersetup
