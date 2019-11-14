FROM debian

RUN apt update && \
    apt install -y curl openssh-server ca-certificates postfix
RUN curl https://packages.gitlab.com/install/repositories/gitlab/gitlab-ce/script.deb.sh

RUN chmod +x script.deb.sh && ./script.sh
RUN  apt-get install -y gitlab-ce && tzdata

EXPOSE 443 80 22

