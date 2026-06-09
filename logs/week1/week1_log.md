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

## Day 01 ✅
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

## Day 02 ✅
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

## Day 03 ✅
오늘 한 것:
- `sudo usermod -aG docker dayeon` → sudo 없이 docker 사용 가능
- nginx 컨테이너 백그라운드 실행 (`docker run -d -p 8080:80 nginx`)
- 브라우저에서 `192.168.45.94:8080` 접속 → "Welcome to nginx!" 확인
- `docker logs`로 컨테이너 내부 로그 확인
- `docker stop`으로 컨테이너 정상 종료
- Exited (0) vs Exited (137) 차이 이해
- worker process 2개 = 서버 CPU 2코어 자동 감지 확인

막힌 것:
- 없음

내일 할 것:
- Docker Volume 실습 (`docker volume create`, mount)
- `docker network ls` — 네트워크 구조 파악

---

## Day 04
오늘 한 것:

막힌 것:

내일 할 것:

---

## Day 05
오늘 한 것:

막힌 것:

내일 할 것:

---

## Day 06
오늘 한 것:

막힌 것:

내일 할 것:

---

## Day 07 🛌 휴식

---

## 주간 회고
잘 된 것:

아쉬운 것:

다음 주 가져갈 것:
