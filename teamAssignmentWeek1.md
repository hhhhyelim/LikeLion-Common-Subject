
## 웹
#### -거미줄 처럼 연결된 정보 소통 망, World Wide Web
#### -웹 문서를 인터넷 상의 컴퓨터들끼리 주고 받는 네트워크 시스템
#### -웹 문서의 각 페이지는 하이퍼링크로 상호 연결됨
#
### 동작원리
#### - 서버와 클라이언트로 동작되는 http 모델
#
## HTTP
#### -리소스들을 가져올 수 있도록 해주는 텍스트 기반의 통신 규약 프로토콜
#### -TCP/IP를 이용하는 응용 프로토콜 
  +)TCP/IP는 네트워크 프로토콜 스위트로, 온라인상의 안전하고 효율적인 데이터 전송의 필수 요건을 정의
#### - 비 연결성 프로토콜
#### - HTTP메시지는 서버와 클라이언트에 의해 해석
#
## 웹 서버
#### -하드웨어 : 웹 사이트의 컴포넌트 파일들을 저장하는 컴퓨터
#### -소프트웨어 : 사용자가 어떻게 호스트 파일들에 접근하는지 관리
#### -정적 웹서버 : HTTP 서버 (소프트웨어)가 있는 컴퓨터(하드웨어)로 구성
#### -동적 웹서버 : 추가적인 소프트웨어(애플리케이션 서버와 데이터베이스...)로 구성
#
## 쿠키
#### -정보 저장 용도
#### -도메인에 따라 제한 (ex)유튜브의 쿠키는 유튜브 에서만)
#### -유효기간 있음
#
## 세션 
#### -클라이언트가 재접속 했을 때 클라이언트를 구분할 수 있는 수단
+)http 특성상 요청이 끝나면 누가 접속했는지 잊음
#
#### -서버의 메모리 내부에 저장이 되기에 세션의 양이 많아지면 메모리에 부하가 걸릴 수 있음
#### -서버를 여러대로 확장 및 분산 시 세션을 분산시키는 기술 또한 따로 설계 필요함


# Tokens
#### -쿠키는 브라우저에서만 사용되지만 토큰은 서버로 보내짐
#### -서버가 아닌 클라이언트에 저장됨(세션의 단점을 보완)
# JWT
#### -인증에 필요한 정보들을 토큰에 담아 암호화
#### -세션 DB를 가질 필요 없음(메모리 부하 방지)
#### -토큰을 통해 세션관련 정보를 검증