---
title: "게임 클라이언트 작업 정의"
date: 2018-08-07T08:30:11-07:00
weight: 13
---

세번째 작업 정의는 tic-tac-toe-client 를 만듭니다.
이 작업은 간단한 웹 호스팅으로 FARGATE타입으로 생성하겠습니다.

* **launch type**: FARGATE
* **Task Definition Name**: tic-tac-toe-client
* **Task Role**: tic-tac-toe-task-role
* **Task execution role**: tic-tac-toe-task-role
* **Task memory**: 0.5GB
* **Task CPU**: 0.25 vCPU


**Add container**를 선택합니다.

* **Container name**: tic-tac-toe-client
* **Image**: tic-tac-toe-client 컨테이너 이미지 이름과 태그를 넣습니다. 100280XXXXXX.dkr.ecr.us-west-2.amazonaws.com/tic-tac-toe-client:latest 의 형식입니다.
* **Port mappings**: 80
* **HELATHCHECK** 항목은 입력하지 않습니다.
* **Log configuration**/**Auto-configure CloudWatch Logs**: 활성화

**Add**를 선택합니다. 이미 한번 적용했다면 버튼 이름은 **Update**로 변경됩니다.

**Create** 를 선택해서 작업을 만듭니다.