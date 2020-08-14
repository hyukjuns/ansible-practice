# Install Docker Engine in CentOS7 and Ubuntu
# And Run hello-world container for test
## Case 1. Create Playbook for install docker engine
CentOS 와 Ubuntu 를 구별하여 설치하기 위해 block과 when절을 사용하였고, when절에 facts 변수로 OS를 분류함
## Case 2. Create Roles for Simple Playbook
docker 라는 role을 만들어서 1번 playbook의 tasks를 분리한다. 그 후 main tasks에서 OS에 따라 tasks를 include하여 playbook을 심플하게 구성함