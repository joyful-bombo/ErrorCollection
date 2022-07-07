# ErrorCollection

## Tomcat 서버 관련
- **8080 포트 충돌시 오류 해결**
  ```bash
  lsof -i :8080(포트번호)
  
  
  COMMAND  PID     USER   FD   TYPE             DEVICE SIZE/OFF NODE NAME
  node    1234     bombo  15u  IPv4 0x1f23462a48d69d65      0t0  TCP localhost:cslistener (LISTEN)

  
  kill -9 Pid
  ```
