# Ansible
Ansible 사용 연습

## Skills
- role
- block
- when
- include_tasks, include_vars
- group_vars, host_vars
- handler
- etc...

## Deploy Scenarios
### scenario1: Install Docker in CentOS7 and Ubuntu 18.04
Link: [install docker][linkto1]

[linkto1]: https://github.com/namhj94/Ansible/tree/master/install_docker

### scenario2: HAProxy Configuration by ansible
Link: [HAProxy][linkto2]

[linkto2]: https://github.com/namhj94/Ansible-HAProxy

## Ansible 공부순서
1. Ansible 이란
2. Ansible 설치
    - Ansible 구성요소

    > 인벤토리, 컨트롤노드, 관리노드, 플러그인

3. 설정파일(ansible.cfg)
    - default 영역
    - privilege_escalation 영역
    - 기타 다른 영역
4. 인벤토리
    - 정적인벤토리
    - 동적인벤토리
5. 일회성 명령어 실행(ansible ad hoc)
    - 모듈의 사용법
    - ping모듈 사용
    - command 모듈 사용
    - 인증관련 옵션들
6. 플레이북
    - yaml
    - 간단한 플레이북 작성
    - 핸들러
7. 변수
    - 변수 소개
    - 변수의 범위(글로벌/플레이/인벤토리)
    - 리스트 변수
    - 해시 변수
    - 결합된 변수(리스트+해시)
    - 등록된 변수
    - 팩트
8. 조건문과 박복문
    - when
    - loop
9. 파일 배포 모듈
    - copy
    - template
10. include 와 import
    - 변수 (include_vars)
    - 작업 (include_tasks / import_tasks)
    - 플레이북 (import_playbook)
11. Role
    - Role의 구조
    - ansible-galaxy
    - 변수 우선순위
    - 예시 Role 분석
12. 오류제어
    - ingnore_erros
    - block과 block rescue
    - force_handler
