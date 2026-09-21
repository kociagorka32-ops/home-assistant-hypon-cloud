FROM ghcr.io/home-assistant/base:latest

RUN apk add --no-cache mosquitto-clients jq curl

COPY run.sh /
COPY scripts/ /scripts/

RUN chmod a+x /run.sh /scripts/*.sh

CMD [ "/run.sh" ]
