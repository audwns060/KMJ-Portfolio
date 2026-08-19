# KMJ Portfolio

> Infrastructure · Cloud · Security

Terraform 기반 AWS 인프라 구축과 Suricata·ELK 기반 IDS 모니터링 환경 구축 프로젝트를 정리한 포트폴리오입니다.

---

## 📘 Portfolio

### 🔹 AWS + IDS 통합 포트폴리오
두 프로젝트의 설계 과정, 구축 내용 및 결과를 하나의 문서로 정리했습니다.

📄 [AWS · IDS 프로젝트 포트폴리오](./AWS_IDS%20포트폴리오.pdf)
---

## ☁️ Project 01. Terraform 기반 AWS 인프라 구축

**Terraform을 활용하여 재현 가능한 AWS 웹 서비스 인프라를 코드 기반으로 구축한 프로젝트**

### 주요 구성
- Terraform 기반 IaC
- VPC / Public·Private Subnet 구성
- EC2 기반 웹 서비스 구축
- ALB · Auto Scaling 기반 트래픽 분산 및 확장
- RDS 기반 데이터베이스 구성
- AWS WAF 기반 웹 요청 보호
- CloudWatch 기반 모니터링

**Tech Stack**  
`Terraform` `AWS` `VPC` `EC2` `RDS` `ALB` `Auto Scaling` `WAF` `CloudWatch`

📄 [AWS 포트폴리오](./AWS%20포트폴리오.pdf)

---

## 🛡️ Project 02. Suricata · ELK 기반 IDS 모니터링 환경 구축

**웹 공격 탐지부터 이벤트 수집·저장·분석·시각화까지 연결한 IDS 모니터링 환경 구축 프로젝트**

### 주요 구성
- Outside · Inside · DMZ 네트워크 영역 구성
- Suricata 기반 웹 공격 탐지 및 Rule 작성
- Filebeat 기반 보안 이벤트 전달
- Elasticsearch 다중 노드 기반 이벤트 저장 및 검색
- Kibana Dashboard 기반 로그 분석·시각화
- SQL Injection · XSS · Brute Force 공격 시나리오 검증

**Tech Stack**  
`Rocky Linux` `Suricata` `Filebeat` `Elasticsearch` `Kibana` `GNS3`

📄 [IDS 포트폴리오](./IDS%20포트폴리오.pdf)

---

## 📂 Original Project Files

프로젝트 수행 당시 작성한 원본 자료입니다.

- 📄 AWS 프로젝트 원본
- 📄 Suricata · ELK IDS 프로젝트 원본

---

## 🔗 Contact

- GitHub: audwns060
- E-mail: audwns060@naver.com
