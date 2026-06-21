# KMJ-Portfolio
my-portfolio
# 🚨 Suricata IDS Monitoring System

> GNS3 기반 네트워크 환경에서 Suricata IDS와 ELK Stack을 활용하여 실시간 침입 탐지 및 로그 분석 시스템을 구축한 프로젝트

---

## 📌 프로젝트 개요

본 프로젝트는 GNS3 기반 가상 네트워크 환경에서 Suricata IDS와 ELK Stack을 활용하여 실시간 침입 탐지 및 로그 분석 환경을 구축한 프로젝트입니다.

OSPF, VLAN, VRRP를 활용하여 네트워크를 설계하고 DMZ 영역에 WordPress, DVWA, DNS 서버를 배치하여 실제 공격 시나리오를 생성하였습니다.

또한 Suricata IDS를 통해 SQL Injection, XSS, Brute Force 공격을 탐지하고 Elasticsearch와 Kibana를 활용하여 보안 이벤트를 실시간으로 시각화하였습니다.

---

## 🛠 개발 환경 및 기술 스택 (Tech Stacks)

| 분류 | 기술 스택 |
|---|---|
| Network | GNS3, OSPF, VLAN, VRRP |
| Security | Suricata IDS |
| Monitoring | Elasticsearch, Kibana, Filebeat |
| Server | Rocky Linux 9 |
| Web Service | WordPress, DVWA |
| DNS | BIND DNS Master / Slave |

---

## 🏗 네트워크 아키텍처 (Network Topology)

<img width="1175" height="685" alt="화면 캡처 2026-06-21 235604" src="https://github.com/user-attachments/assets/12eedb77-1347-465c-8482-caf6bae34345" />

---

## 🌐 OUTSIDE (외부망)

### 구성 요소

- Internet Router
- R1
- R2

### 구현 내용

- 외부 인터넷 연결 구간 구성
- R1, R2 기반 외부 라우팅 경로 구성
- OSPF 기반 동적 라우팅 설정
- 기본 경로(Default Route)를 통한 외부망 통신 구현

---

## 🔥 FIREWALL (방화벽 이중화 영역)

### 구성 요소

- FW1
- FW2

### 구현 내용

- FW1, FW2 이중화 구성
- VRRP 기반 Gateway 이중화 구현
- Active / Standby 구조를 통한 장애 대응 구성
- 내부망과 DMZ 구간 간 트래픽 경로 제어

---

## 🖥 INSIDE (내부망)

### 구성 요소

- SW1
- SW2
- SW3
- PC1
- PC2

### 구현 내용

- 내부 사용자망 구성
- VLAN 기반 네트워크 분리
- 내부 PC 구간 통신 확인
- Gateway 이중화 환경에서 내부망 통신 검증

---

## 🌍 DMZ (서비스 영역)

### 구성 요소

- WordPress Server
- DVWA Server
- DNS Master Server
- DNS Slave Server
- Suricata IDS Server
- Elasticsearch Cluster
- Kibana Server
- Filebeat

### 구현 내용

- WordPress 웹 서버 구축
- DVWA 취약점 테스트 서버 구축
- DNS Master / Slave 서버 구축
- Suricata IDS 기반 패킷 탐지 환경 구성
- Elasticsearch 3 Node Cluster 구축
- Filebeat를 통한 로그 수집 및 전달
- Kibana Dashboard를 통한 보안 이벤트 시각화

---

## 👨‍💻 담당 역할 (My Contribution)

### Server

- DNS Master / Slave 구축
- WordPress 웹 서버 구축
- DVWA 취약점 테스트 서버 구축

### Monitoring

- Elasticsearch Multi Node Cluster 구축
- Filebeat 연동
- Kibana Dashboard 구성

### Network

- GNS3 기반 네트워크 구성 참여
- VLAN, OSPF, VRRP 구성 검증
- 내부망 / 외부망 / DMZ 통신 테스트

### Documentation

- 프로젝트 계획서 작성
- 결과 보고서 작성
- 최종 발표 진행

---

## 🚨 공격 탐지 시나리오

### 1. ICMP Ping Detection

- ICMP 패킷 탐지
- Suricata Alert 생성
- Kibana Dashboard 시각화

### 2. SQL Injection Detection

```sql
' OR 1=1 --
```

- SQL Injection 공격 수행
- Suricata Rule 기반 탐지
- Elasticsearch 로그 저장
- Kibana Dashboard 시각화

### 3. XSS Detection

```html
<script>alert('xss')</script>
```

- XSS Payload 수행
- Suricata Rule 기반 탐지
- Elasticsearch 로그 저장
- Kibana Dashboard 시각화

### 4. Brute Force Detection

```text
admin
admin123
password
123456
```

- 반복 로그인 시도 탐지
- Alert 생성
- Kibana Dashboard 시각화

---

## 📊 프로젝트 성과

- OSPF 기반 동적 라우팅 구성
- VLAN 기반 네트워크 분리
- VRRP 기반 Gateway 이중화
- DNS Master / Slave 구축
- WordPress 웹 서버 구축
- DVWA 취약점 테스트 환경 구축
- Suricata IDS 구축
- SQL Injection 탐지
- XSS 탐지
- Brute Force 탐지
- Elasticsearch Multi Node Cluster 구축
- Kibana Dashboard 시각화

---

## 📚 Learned

- 네트워크 설계와 서버 구축의 연계 이해
- IDS 기반 침입 탐지 프로세스 학습
- ELK Stack 기반 로그 수집 및 분석 경험
- 보안 이벤트 시각화 경험
- 팀 프로젝트 협업 및 문서화 경험

---

## ⭐ Result

실제 네트워크 환경과 유사한 구조를 설계하여 Network, Server, Security, Monitoring 전 과정을 경험하였습니다.

Suricata IDS와 ELK Stack을 연동하여 공격 이벤트를 수집, 분석, 시각화하는 보안 모니터링 환경을 구현하였습니다.
