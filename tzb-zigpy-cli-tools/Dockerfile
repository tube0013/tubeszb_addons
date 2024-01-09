ARG BUILD_FROM
ARG BUILD_ARCH

FROM $BUILD_FROM


RUN \
    set -x \
    && apk add --no-cache \
        py3-pip \
        python3 \
        git \
    && pip3 uninstall -y setuptools \
    && pip3 install zigpy-cli

COPY rootfs /

# use s6-overlay as init system
WORKDIR /
ENTRYPOINT ["/init"]