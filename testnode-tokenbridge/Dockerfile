FROM node:16-bullseye-slim
RUN apt-get update && \
    apt-get install -y git docker.io
WORKDIR /workspace
RUN git clone -b fix_eip1559 https://github.com/s7v7nislands/arbitrum-sdk.git ./ 
RUN yarn install
ENTRYPOINT ["yarn"]
