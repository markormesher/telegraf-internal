FROM telegraf
COPY telegraf.conf /etc/telegraf/
ARG HOSTNAME
RUN [ -n "${HOSTNAME}" ] || exit 1
RUN sed -i "s/CHANGE_THE_HOSTNAME/${HOSTNAME}/g" /etc/telegraf/telegraf.conf
