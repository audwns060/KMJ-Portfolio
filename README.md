# KMJ-Portfolio
my-portfolio
# 🚨 Suricata IDS Monitoring System

> GNS3 기반 네트워크 환경에서 Suricata IDS와 ELK Stack을 활용하여 실시간 침입 탐지 및 로그 분석 시스템을 구축한 프로젝트

![Linux](https://img.shields.io/badge/Linux-Rocky9-green)
![ELK](https://img.shields.io/badge/ELK-Stack-yellow)
![Suricata](https://img.shields.io/badge/IDS-Suricata-red)
![Network](https://img.shields.io/badge/Network-OSPF%20%7C%20VLAN%20%7C%20VRRP-blue)

---

# 📌 Project Overview

본 프로젝트는 네트워크 트래픽과 웹 로그를 수집하여 실시간 침입 탐지 및 분석 환경을 구축하는 것을 목표로 진행되었습니다.

GNS3 기반 가상 네트워크 환경에서 OSPF, VLAN, VRRP를 이용한 네트워크를 설계하고 WordPress 및 DVWA 서버를 구축하여 실제 공격 시나리오를 생성하였습니다.

수집된 로그는 Filebeat를 통해 Elasticsearch로 전달하고 Kibana Dashboard를 통해 시각화하였습니다.

또한 SQL Injection, XSS, Brute Force 공격 탐지 규칙을 적용하여 보안 이벤트를 분석하였습니다.

---

# 📅 Project Period

2025.12.17 ~ 2025.12.31

---

# 🛠 Tech Stack

## Network

- GNS3
- OSPF
- VLAN
- VRRP

## Security

- Suricata IDS
- Custom Detection Rules

## Monitoring

- Elasticsearch
- Kibana
- Filebeat

## Server

- Rocky Linux 9
- WordPress
- DVWA
- Bind DNS

---

# 🏗 Architecture

text
Internet
   │
 ┌─┴─┐
R1   R2
 │   │
FW1 FW2
   │
 DMZ
 ├─ WordPress
 ├─ DVWA
 ├─ DNS Master
 ├─ DNS Slave
 ├─ Suricata
 └─ Elasticsearch Cluster

INSIDE
 ├─ PC1
 └─ PC2

> <img width="1175" height="685" alt="화면 캡처 2026-06-21 235604" src="https://github.com/user-attachments/assets/65ce1143-66c7-418f-b4d8-4e2cd9e8283e" />

---

# 👨‍💻 My Contribution

## Network

- VLAN 기반 네트워크 분리
- OSPF 동적 라우팅 구성
- VRRP 기반 Gateway 이중화 구현

## Server

- DNS Master / Slave 구축
- WordPress 구축
- DVWA 구축

## Monitoring

- Elasticsearch Multi Node Cluster 구축
- Filebeat 연동
- Kibana Dashboard 구성

## Documentation

- 프로젝트 계획서 작성
- 결과 보고서 작성
- 최종 발표 진행

---

# 🚀 Key Achievements

### Network

- OSPF 기반 동적 라우팅 구성
- VLAN 기반 네트워크 분리
- VRRP 기반 Gateway 이중화

### Security

- Suricata IDS 구축
- SQL Injection 탐지
- XSS 탐지
- Brute Force 탐지

### Monitoring

- Elasticsearch 3 Node Cluster 구축
- Filebeat 연동
- Kibana Dashboard 시각화

---

# 🔍 Attack Detection Scenario

## ICMP Ping Detection

```text
Attacker
   ↓
 ICMP Request
   ↓
 Suricata Alert
   ↓
 Elasticsearch
   ↓
 Kibana Dashboard
```

---

## SQL Injection Detection

```sql
' OR 1=1 --
```

- Suricata Rule 기반 탐지
- Elasticsearch 저장
- Kibana Dashboard 시각화

---

## XSS Detection

```html
<script>alert('xss')</script>
```

- Suricata Rule 기반 탐지
- Elasticsearch 저장
- Kibana Dashboard 시각화

---

## Brute Force Detection

```text
admin
admin123
password
123456
```

- 반복 로그인 시도 탐지
- Alert 생성
- Dashboard 시각화

---

# 📊 Dashboard

<img width="1176" height="581" alt="화면 캡처 2026-06-21 235539" src="https://github.com/user-attachments/assets/6f298b80-c6bc-4ddd-b7bc-c07940c08d96" />

---

# 📚 Learned

- 네트워크 설계와 서버 구축의 연계 이해
- IDS 기반 침입 탐지 프로세스 학습
- ELK Stack 기반 로그 수집 및 분석 경험
- 보안 이벤트 시각화 경험
- 팀 프로젝트 협업 및 문서화 경험

---

# 📎 Reference

- Suricata
- Elasticsearch
- Kibana
- Filebeat
- GNS3

---

# ⭐ Result

실제 네트워크 환경과 유사한 구조를 설계하여

- Network Engineering
- Server Administration
- Security Monitoring
- Log Analysis

전 과정을 경험하였으며,

실시간 침입 탐지 및 보안 모니터링 환경을 구현하였습니다.
