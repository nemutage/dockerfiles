FROM centos:8

RUN yum -y update \
    && yum -y install openssh-server \ 
    && yum clean all


# sshサーバ起動
# systemctl start sshd.service

# sshサーバ停止
# systemctl start sshd.service