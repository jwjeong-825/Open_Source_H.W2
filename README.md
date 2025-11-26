 ###### 리눅스 명령어 조사

### **<목차>**
1. top
2. ps
3. jobs
4. kill
5. 명령어 비교표


## 1. top - 실시간 프로세스 모니터링
- 명령어 설명<br>
top은 리눅스의 ‘작업 관리자(Task Manager)’와 동일한 기능을 한다.
CPU, 메모리 사용량, 실행 중인 프로세스를 실시간(real-time) 으로 확인할 수 있다.


- 사용법
```bash
$ top 
```

- 화면 구성 요소
  
| 항목      | 설명           |
| --------- | -------------- |
| PID       | 프로세스 ID    |
| USER      | 실행한 사용자  |
| %CPU      | CPU 사용량     |
| %MEM      | 메모리 사용량  |
| TIME+     | 누적 CPU 시간  |
| COMMAND   | 실행된 명령어  |


- 자주 사용하는 단축키
   
 q : top 종료

P : CPU 사용량 기준 정렬

M : 메모리 사용량 기준 정렬

k : 특정 프로세스 종료

h : 도움말

 
 - 사용예시
 <img width="958" height="246" alt="image" src="https://github.com/user-attachments/assets/7b07b07f-bd2e-443e-97bd-2eb467999faa" />


 ## 2. ps - 정적인 프로세스 정보 확인
- 명령어 설명<br>
ps는 ‘현재 시점’의 프로세스 정보를 한 번만 출력하는 명령어이다.
top이 ‘실시간’이라면 ps는 ‘스냅샷(snapshot)’.

- 사용법
```bash
$ ps -e / -f / aux
```

- 화면 구성 요소

| 항목        | 설명                                             |
|-------------|--------------------------------------------------|
| USER        | 프로세스를 실행한 사용자                          |
| PID         | 프로세스 ID                                       |
| PPID        | 부모 프로세스 ID                                  |
| %CPU        | CPU 사용량                                        |
| %MEM        | 메모리 사용 비율                                  |
| VSZ         | 가상 메모리 사용량(단위: KB)                      |
| RSS         | 실제 메모리 사용량(Resident Set Size)             |
| TTY         | 연결된 터미널                                     |
| STAT        | 프로세스 상태 (S, R, D, T 등)                     |
| START       | 프로세스 시작 시간                                |
| TIME        | 누적 CPU 사용 시간                                |
| COMMAND     | 실행한 명령어                                     |


- 주요 옵션
  
| 명령어    | 설명                                  |
|-----------|----------------------------------------|
| ps -e     | 모든 프로세스 출력                     |
| ps -f     | Full Format 형태로 상세 정보 표시      |
| ps aux    | 가장 많이 사용하는 전체 프로세스 정보  |


- 사용예시
  <img width="931" height="375" alt="image" src="https://github.com/user-attachments/assets/6aa8bbcb-4a18-4e72-bc86-7c23eedd84c6" />




