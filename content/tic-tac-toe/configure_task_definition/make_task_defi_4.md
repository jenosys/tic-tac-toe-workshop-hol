---
title: "대시보드 작업 정의"
date: 2018-08-07T08:30:11-07:00
weight: 14

---

마지막으로 만들 작업 정의는 dashboard 를 만듭니다.
앞서 matchmaker 작업 정의를 참고하여 아래 항목을 적용한 작업 정의를 만들면 됩니다. 

* **launch type**: FARGATE
* **Task Definition Name**: dashboard
* **Task Role**: tic-tac-toe-task-role
* **Task execution role**: tic-tac-toe-task-role
* **Task memory**: 0.5GB
* **Task CPU**: 0.25 vCPU


**Add container**를 선택합니다.

* **Container name**: dashboard
* **Image**: dashboard 컨테이너 이미지 이름과 태그를 넣습니다. 100280XXXXXX.dkr.ecr.us-west-2.amazonaws.com/dashboard:latest 의 형식입니다.
* **Port mappings**: 80
* **HELATHCHECK** 항목은 입력하지 않습니다.
* **Log configuration**/**Auto-configure CloudWatch Logs**: 활성화 

**Add**를 선택합니다. 이미 한번 적용했다면 버튼 이름은 **Update**로 변경됩니다.

**Create** 를 선택해서 작업을 만듭니다.