FROM node:23-bookworm

COPY ./services/node/scripts/entrypoint.sh /docker-scripts/entrypoint.sh
RUN chmod +x /docker-scripts/entrypoint.sh

RUN apt-get update && \ 
    apt-get install -y --no-install-recommends \
    ca-certificates

RUN npm install -g pnpm

ENTRYPOINT ["/docker-scripts/entrypoint.sh"]
WORKDIR /home/node/app

CMD ["node","/home/node/app/main.mjs"]