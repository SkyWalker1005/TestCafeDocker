FROM testcafe/testcafe
# See https://github.com/DevExpress/testcafe/tree/master/docker

USER root

ENV LANG C.UTF-8
ARG USER=testcafeuser
ENV HOME /home/$USER

# install sudo as root
RUN apk add --update sudo

# add new user
RUN adduser -D $USER \
        && echo "$USER ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/$USER \
        && chmod 0440 /etc/sudoers.d/$USER

USER $USER
WORKDIR $HOME

#Install git
RUN sudo apk update && \
    sudo apk add git

#Create user directory
RUN sudo mkdir $HOME/TestCafeProjects
ENTRYPOINT []
