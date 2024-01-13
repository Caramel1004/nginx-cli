# nginx-cli
### nginx 명령어 정리 <br>
Nginx는 다양한 명령어를 제공하여 설정 관리 및 서버 운영을 지원합니다. 아래는 일반적으로 사용되는 Nginx 명령어 몇 가지입니다. 이 명령어들은 주로 Unix/Linux 환경에서 사용됩니다.

#### 1. Nginx 시작 및 종료:

- sudo service nginx start: Nginx 시작
- sudo service nginx stop: Nginx 종료
- sudo service nginx restart: Nginx 재시작
- sudo service nginx reload: Nginx 설정 재적용 (재시작보다 경량적)

#### 2. Nginx 설정 파일 관련:

- nginx -t 또는 sudo nginx -t: Nginx 설정 파일의 유효성 검사
- sudo nginx -s reload: Nginx 설정 파일 재적용 (reload와 동일)

#### 3. 프로세스 관리:

- ps aux | grep nginx: Nginx 프로세스 확인
- sudo pkill nginx: 모든 Nginx 프로세스 강제 종료
#### 4. 로그 파일 관련:

- 에러 로그: /var/log/nginx/error.log
- 접근 로그: /var/log/nginx/access.log
#### 5. 서버 정보 확인:

- nginx -v 또는 nginx -V: Nginx 버전 확인
- nginx -h: 사용 가능한 명령어 옵션 확인
#### 6. 기타:

- sudo systemctl status nginx: Nginx 서비스 상태 확인 (systemd 사용 시)
- sudo systemctl enable nginx: 부팅 시 자동으로 시작하도록 설정 (systemd 사용 시)
