FROM nginx:alpine
ARG USERNAME=vscode
ARG USER_UID=1000
ARG USER_GID=$USER_UID
RUN addgroup -g $USER_GID -S $USERNAME && adduser -u $USER_UID -s /bin/sh -S -G $USERNAME $USERNAME
#USER $USERNAME
COPY default.conf /etc/nginx/conf.d/default.conf
WORKDIR /home/$USERNAME

