# FROM node:14.4.0-alpine 使用不可
FROM node:16.15.1-alpine

ARG WORKDIR
ARG CONTAINER_PORT

ENV HOME=/${WORKDIR} \
    LANG=C.UTF-8 \
    TZ=Asia/Tokyo \
    HOST=0.0.0.0

# ENV check（このRUN命令は確認のためなので無くても良い）
RUN echo ${HOME}
RUN echo ${CONTAINER_PORT}

WORKDIR ${HOME}

#  公開用ポート番号を指定
# http;//localhost(0,0,0,0):3000が紐付けられている
EXPOSE ${CONTAINER_PORT}
