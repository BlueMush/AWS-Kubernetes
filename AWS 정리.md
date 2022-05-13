AWS 정리
==============

## 목차
1. [CloudService란](#1-CloudService)
      * [서비스유형](#서비스유형)
2. [AWS란](#2-AWS)
      * [EKS](#EKS)
      * [EC2](#EC2)
      * [ELB](#ELB)
      * [VPC](#VPC)


---
## 1. CloudService
### 클라우드 서비스
* 인터넷 기반의 컴퓨팅
* 인터넷 통신망 어딘가에 있는 컴퓨팅 자원을 가져다 쓸 수 있는 서비스
* 서버를 직접 구매해도 되지않아 초기세팅 비용절감에 도움을 줌

### Public Cloud
* 인터넷에 접속 가능한 모든 사용자를 위한 클라우드 서비스 모델
* 데이터나 기능, 서버 같은 자원은 사용자 별로 권한관리되어 서비스 사용자 간 간섭이 없음

### Private Cloud
* 제한된 네트워크 상에서 특정 기업이나 특정 사용자만을 대상으로 하는 클라우드 서비스
* 서비스의 자원과 데이터는 기업 내부에 저장됨
* 보안성 우수
* 개별 고객의 상황에 맞게 커스터마이징 가능

### 서비스유형
### IaaS
* Infrastructure as a Service
* 기존 서버 호스팅보다 하드웨어 확장성이 좋고 탄력적임
* Paas, SaaS의 기반이 되는 기술


### PaaS
* Platform as a Service
* 가상화된 클라우드 위에 개발 환경을 미리 구축하여 서비스 형태로 제공
* 운영체제, 미들웨어, 런타임 등을 미리 구축하여 제공

### SaaS
* Service as a Service
* 클라우드 인프라 위에 소프트웨어를 탑재해 서비스로 제공

![image](https://user-images.githubusercontent.com/37949471/168026157-5a6d002f-59f0-41dc-81b1-ee8763ecba6d.png)

---
## 3. AWS
### Amazon Web Service
* 아마존에서 제공하는 클라우드 서비스

### EKS
* Elastic Kubernetes Service
* AWS에서 만든 관리형 쿠버네티스 서비스
* EKS를 사용하면 쿠버네티스 마스터노드 구성을 할 필요없이 AWS에서 관리해줌

### EC2
* Elastic Compute Cloud
* 크기 조정가능한 가상의 컴퓨터를 클라우드로 제공해주는 서비스

### ELB
* Elastic Load Balancer
* 로드밸런서의 주요 기능은 한 서버에 부하가 몰리지 않게 분산시켜주는 역할
![image](https://user-images.githubusercontent.com/37949471/168220341-9c86f420-67e9-46d6-b508-4bdc450944ae.png)
* L4 IP, Port 기준으로 스케줄링 알고리즘을 통해 부하를 분산
* L7 IP, Port + URI, Payload, Http Header, Cookie를 추가로 산정하여 부하를 분산함


