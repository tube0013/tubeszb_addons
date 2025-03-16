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
    && pip3 install gpiod intelhex pyserial python_magic scripttest setuptools \
    && python3 -m pip install git+https://github.com/mercenaruss/cc1352-flasher.git

COPY rootfs /

# use s6-overlay as init system
WORKDIR /
ENTRYPOINT ["/init"]
