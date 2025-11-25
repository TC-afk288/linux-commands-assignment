# Linux Commands Assignment
20253008 최태민 오픈소스SW개론 과제2

---

## 1. top
- 시스템 상태 모니터링 명령어
- CPU, 메모리 사용량, 프로세스 정보 등을 실시간으로 보여줌

### 주요 옵션
| 옵션 | 설명 |
|------|------|
| -n 1 | 1회만 실행 후 종료 |
| -b   | 배치 모드, 출력 내용을 다른 명령어나 파일로 전달 가능 |

### 예시 출력
top -n 1
Tasks: 120 total, 2 running, 118 sleeping, 0 stopped, 0 zombie
%Cpu(s): 3.0 us, 1.0 sy, 0.0 ni, 95.0 id, 1.0 wa, 0.0 hi, 0.0 si, 0.0 st
Mem: 8175244k total, 246812k used, 7928432k free, 12344k buffers


---

## 2. ps
- 현재 시스템에서 실행 중인 프로세스를 확인하는 명령어

### 주요 옵션
| 옵션 | 설명 |
|------|------|
| aux  | 모든 사용자 프로세스 전체 표시 |
| -ef  | 표준 전체 포맷으로 프로세스 표시 |

### 예시 출력
ps aux
USER PID %CPU %MEM VSZ RSS TTY STAT START TIME COMMAND
root 1 0.0 0.1 22568 1204 ? Ss 09:00 0:01 init


---

## 3. jobs
- 현재 세션에서 실행 중인 백그라운드 작업을 확인

### 예시 출력
jobs
[1]+ Running sleep 100 &
[2]- Stopped nano


---

## 4. kill
- 프로세스를 종료하는 명령어

### 사용 방법
- 예시: `kill 1234` → PID 1234인 프로세스를 종료

### 주요 옵션
| 옵션 | 설명 |
|------|------|
| -9   | 강제 종료(SIGKILL) |
| -15  | 정상 종료(SIGTERM, 기본값) |
