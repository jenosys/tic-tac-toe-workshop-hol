---
title: "ECS 클러스터 생성하기"
chapter: false
weight: 2
---

## ECS 클러스터 생성하기

1. 상단의 왼쪽의 **Services** 메뉴를 통해 ECS로 넘어갑니다.
1. 상단 우측 메뉴에서 현재 리전이 **Oregon**인지 확인합니다.
1. 왼쪽 사이드 메뉴에서 **Cluster**를 선택하고 **Create Cluster**를 선택합니다.
1. 클러스터 종류는 **EC2 Linux + Networking** 을 선택하고 **Next step**을 선택합니다.
![Example Service](/images/tic-tac-toe/cluster-build-1.png)
1. **Cluster name**에 tic-tac-toe-cluster 을 입력합니다.
1. **instance configureation**항목에 아래 내용을 입력합니다.
 * **EC2 instance type**: m5.large
 * **Number of instances**: 3
 * **key pair**: tic-tac-toe 
 * 기타 항목은 기본값으로 둡니다.
![Example Service](/images/tic-tac-toe/cluster-build-2.png)

1. **Networking**항목 아래 내용으로 입력합니다.
 * **VPC**: Create VPC 선택
 * **Container instance IAM role**: tic-tac-toe-ecs-role 선택
 * 하단의 **CloudWatch Container Insights** 항목 선택 확인
 * 기타 항목은 기본값으로 둡니다.
1. 하단의 **Create**를 선택하여 다음으로 넘어갑니다.
![Example Service](/images/tic-tac-toe/cluster-build-3.png)

1. 클러스터와 VPC가 생성되는데 시간이 조금 필요합니다.<br>
만들어진 VPC 아이디를 기억하고 있으면 편리합니다.

![Example Service](/images/tic-tac-toe/cluster-build-4.png)
