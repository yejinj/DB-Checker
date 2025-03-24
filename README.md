## Toy Project: Event Managment System

## 소개
대학교의 이벤트 관리 및 참여자 체크인 시스템입니다. 관리자가 이벤트를 생성하고 참여자들의 출석/수령 여부를 실시간으로 관리할 수 있습니다.
프로젝트에서 기획 및 프론트엔드 개발을 맡아 진행하였습니다.

## 주요 기능
### 1. 이벤트 생성 및 관리
- 이벤트 이름, 내용, 이미지, 종료일 설정
- 이벤트별 고유 해시값 자동 생성
- 잔여 수량 실시간 관리
- 이벤트 활성화/비활성화 상태 관리
- 이벤트 옵션 동적 추가/제거 기능

### 2. 참여자 관리
- 학생 정보(학번, 이름, 사진) 표시
- 실시간 체크인/체크아웃 처리
- 수령 상태 자동 업데이트
- 참여자 검색 및 필터링

### 3. 대시보드
- 이벤트별 참여 현황 파이 차트
- 실시간 잔여 수량 모니터링
- 이벤트 검색 기능

## 기술 스택
- **Frontend**: HTML, CSS, JavaScript
- **Template Engine**: EJS
- **UI 라이브러리**: Font Awesome, AOS
- **차트**: Chart.js

## 실행
1. 저장소 클론
   ```bash
   git clone <repository-url>
   ```
2. 의존성 설치
   ```bash
   npm install
   ```
3. 환경 변수 설정
   ```bash
    DB_HOST=localhost
    DB_USER=root
    DB_PASSWORD=your_password
    DB_DATABASE=checker_db
   ```
4. 서버 실행
   ```bash
   npm start
   ```

## 구조
- **메인 페이지**: `/`
- **관리자 페이지**: `/admin`
- **이벤트 상세 페이지**: `/eventView/:eventHash`

## 보안
- 관리자 인증 시스템
- 이벤트 해시 기반 접근 제어
- XSS 방지
- 파일 업로드 제한
