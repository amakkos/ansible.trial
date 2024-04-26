FROM python:3.10
RUN pip install ansible firewall
RUN apt-get update
RUN apt-get -y install vim nano openssh-server passwd net-tools firewalld
#RUN ssh-keygen  -t ed25519 -P ULYSSYS -f /root/.ssh/id_ed25519
#ADD  ansible_control/id_ed25519* /root/.ssh/
#RUN cp /root/.ssh/id_ed25519.pub /ansible/ansible.pub
#RUN cp /ansible/id_ed25519 /root/.ssh/
#RUN chmod 600 /root/.ssh/id_ed25519
