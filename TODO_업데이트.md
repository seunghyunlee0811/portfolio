# 포트폴리오 업데이트 체크리스트

`index.html`에서 실제 정보로 교체해야 할 부분을 섹션별로 정리했습니다.
각 항목 옆 줄 번호(`Lxxx`)를 참고해서 수정하세요.

## 공통 / 연락처
- [ ] `L425` Email: `seunghyun.lee@email.com` → 실제 이메일 주소
- [ ] `L651` mailto 링크의 이메일도 동일하게 변경
- [ ] `L375`, `L652` GitHub 링크: `https://github.com/username` → 실제 GitHub 계정
- [ ] `L653` LinkedIn 링크: `https://linkedin.com/in/username` → 실제 LinkedIn 계정 (없으면 버튼 자체를 삭제)
- [ ] `L507`,`L535`,`L563` 각 프로젝트의 GitHub/Docs 링크 (`href="#"`로 비어있음) → 실제 저장소/문서 링크

## About (L385-431)
- [ ] `L426` Education: "클라우드 엔지니어링 부트캠프 수료" → 실제 수료 과정명과 일치하는지 확인 (Certifications 섹션과 표현 통일)
- [ ] 자기소개 문단(L394-419) — 현재는 템플릿성 문구("인프라는 보이지 않을 때 가장 잘 작동한다" 등). 본인의 실제 경험/가치관으로 다시 쓸지 결정

## Skills (L433-490)
현재 등록된 스킬 카드: Cloud / Container & Orchestration / IaC & CI/CD / OS & Language / Monitoring
- [ ] 각 chip이 실제로 다뤄본 기술인지 검증 (모르는 기술 제거, 실사용 기술 추가)
  - Cloud: AWS EC2, VPC, S3, RDS, Route 53, CloudFront, IAM, CloudWatch, Lambda
  - Container: Docker, Kubernetes, EKS, Helm, Docker Compose
  - IaC & CI/CD: Terraform, GitHub Actions, Ansible, Jenkins, ArgoCD
  - OS & Language: Linux, Bash, Python, Git, Nginx, MySQL
  - Monitoring: Prometheus, Grafana, CloudWatch, ELK Stack
- [ ] `chip core` 클래스(진하게 표시되는 핵심 기술)가 실제 자신 있는 기술과 일치하는지 재점검
- [ ] 실제로 다뤄본 다른 스킬(예: GCP, Azure, Redis, Kafka, Vault 등)이 있다면 카드/칩 추가

## Projects (L492-587) — 총 3개, 전부 가상 데이터로 보임
### 프로젝트 1: AWS 3-Tier 고가용성 웹 서비스 인프라 (L502-528)
- [ ] 기간 `2026.03 — 2026.05` 실제 기간으로 수정
- [ ] 팀 구성/역할, 설명, 수치(가용성 99.9%, 구축 4h→15m) 실제 값으로 교체 또는 검증
- [ ] 기술 태그(AWS, Terraform, ALB, Auto Scaling, RDS Multi-AZ, CloudWatch) 실제 사용 스택 확인

### 프로젝트 2: Kubernetes 기반 MSA 배포 파이프라인 (L530-556)
- [ ] 기간 `2026.05 — 2026.06` 실제 기간으로 수정
- [ ] 배포 시간(20m→3m), HPA 검증 등 수치 실제 값 확인
- [ ] 기술 태그(Kubernetes, EKS, ArgoCD, Helm, GitHub Actions, Prometheus) 확인

### 프로젝트 3: 온프레미스 → AWS 마이그레이션 시뮬레이션 (L558-583)
- [ ] 기간 `2026.02 — 2026.03` 실제 기간으로 수정
- [ ] 비용 절감(32%), DMS/CDC 관련 내용 실제 값으로 교체
- [ ] 기술 태그 확인

- [ ] 실제로 진행한 다른 프로젝트가 있다면 `<article class="proj reveal">` 블록 추가
- [ ] 프로젝트가 3개보다 적다면(가상 프로젝트 삭제 필요 시) 해당 `<article>` 블록 통째로 제거

## Certifications & Education (L589-640)
- [ ] `L601-604` AWS Certified Solutions Architect – Associate — 취득 여부 및 취득일(`2026.05`) 확인
- [ ] `L607-611` AWS Certified Cloud Practitioner — 취득 여부 및 취득일(`2026.02`) 확인
- [ ] `L614-618` 리눅스마스터 2급 — 취득 여부 및 취득일(`2025.11`) 확인
- [ ] `L625` "클라우드 엔지니어링 전문가 양성과정" — 실제 교육기관명 입력 (`○○교육기관` 채우기), 기간(`2025.12 — 2026.06`) 확인
- [ ] `L632` "○○대학교 ○○학과 졸업" — 실제 학교명/학과명 입력, 재학 기간(`2019.03 — 2025.08`) 확인
- [ ] 없는 자격증/학력 항목은 `<div class="cred">` 블록 삭제

## Hero / 헤더 (L348-383)
- [ ] `L351-352` "구직 중 — 클라우드 엔지니어" 태그 — 현재 구직 상태와 일치하는지 확인
- [ ] `L378-380` 통계: "3+ 인프라 구축 프로젝트", "2 AWS 자격증", "99.9% 목표 가용성" — 실제 프로젝트/자격증 개수와 일치하도록 수정

## Footer (L661)
- [ ] `© 2026 Lee Seunghyun` — 연도 자동 업데이트 여부만 확인 (하드코딩되어 있음)

---
### 우선순위 제안
1. 이메일/GitHub/LinkedIn 등 연락처 — 가장 먼저 실제 값으로 교체 (현재 전부 더미)
2. 자격증/학력의 `○○` 표기 — 미완성 상태이므로 반드시 채우기
3. 프로젝트 3개가 실제 프로젝트인지, 아니면 예시 데이터인지 확인 후 교체/삭제
4. Skills 칩 목록 실사용 기술로 재검증
