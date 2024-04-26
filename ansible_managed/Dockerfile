FROM python:3.10

RUN apt-get update
RUN apt-get -y install openssh-server passwd net-tools firewalld
RUN pip install firewall
RUN useradd -m ansible
RUN mkdir -p  ~ansible/.ssh/
RUN chown ansible  ~ansible/.ssh/
RUN chmod 700  ~ansible/.ssh/
#ADD ansible_control/id_ed25519.pub /home/ansible/.ssh/authorized_keys
#RUN cat /ansible/id_ed25519.pub > ~ansible/.ssh/authorized_keys
#RUN chmod 600 ~ansible/.ssh/authorized_keys
#RUN chown ansible ~ansible/.ssh/authorized_keys
RUN mkdir /run/sshd
RUN /usr/sbin/sshd
