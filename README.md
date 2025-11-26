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
 <img width="1002" height="206" src="https://github.com/user-attachments/assets/03c051af-7ef2-4abf-950e-d3093294989a" />



