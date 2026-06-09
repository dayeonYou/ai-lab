# WEEK 1 — Linux + Docker + Ollama
기간: 2026-06-07 (Day1) ~ 2026-06-13 (Day6) / Day7 휴식

## 이번 주 목표
- 리눅스 서버 운영 감각
- Docker 기본 감각
- Local AI 실행 성공 경험
- CPU inference 체감

## 서버 스펙 (Day1 확인)
- CPU: Intel Pentium G640 2코어 2.80GHz (HT 없음)
- RAM: 7.6GB (가용 6.5GB)
- Disk: 98GB (여유 83GB)
- Swap: 4GB

---

## Day 01 - 2026-06-07 ✅
오늘 한 것:
- Ubuntu apt update/upgrade 완료
- 시스템 정보 확인 (uname, lscpu, free, df)
- htop 설치
- ai-lab 디렉토리 구조 생성

막힌 것:
- 없음

내일 할 것:
- Docker 설치
- hello-world 실행
- image/container 개념 이해

---

## Day 02 - 2026-06-08 ✅
오늘 한 것:
- Docker 설치 (`sudo apt install -y docker.io`) — Docker 29.1.3
- containerd, runc, bridge-utils 같이 설치됨
- 서비스 자동시작 등록 (`sudo systemctl enable --now docker`)
- hello-world 실행 성공 — Docker Hub pull → 컨테이너 생성 → 실행 → 종료 흐름 직접 확인
- `docker ps -a`로 Exited (0) 컨테이너 확인
- IMAGE / CONTAINER / VOLUME / PORT 4대 개념 이해

막힌 것:
- `docker ps -a` permission denied → sudo 없이 실행 불가 (docker 그룹 미추가)

내일 할 것:
- `sudo usermod -aG docker dayeon` 후 재로그인
- nginx 컨테이너 띄우기 + 포트 열어서 직접 접근

---

## Day 03 - 2026-06-09 ✅
오늘 한 것:
- ai-lab/ + onDeviceAI/memory/ 전체 디렉토리 아키텍처 확정
- Claude 메모리 파일 구조 설계 (MEMORY.md, user_profile.md, project_roadmap.md 등)
- Claude Stop 훅 KST 타임스탬프로 수정
- Day 02 내용 github.io 블로그 포스팅 작성

막힌 것:
- 오전 도커 세션 로그 훅으로 미저장 (Claude Desktop 환경이라 훅 미적용)

내일 할 것:
- nginx 컨테이너 실행 + 포트 포워딩 체험
- `usermod -aG docker dayeon` 적용

---

## Day 04 - 2026-06-10
오늘 한 것:

막힌 것:

내일 할 것:

---

## Day 05 - 2026-06-11
오늘 한 것:

막힌 것:

내일 할 것:

---

## Day 06 - 2026-06-12
오늘 한 것:

막힌 것:

내일 할 것:

---

## Day 07 - 2026-06-13 🛌 휴식

---

## 주간 회고
잘 된 것:

아쉬운 것:

다음 주 가져갈 것:
