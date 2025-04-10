## HTTPS
### HTTP
- HTTP (Hypertext Transfer Protocol)는 클라이언트와 서버 간 통신을 위한 통신 규약이다.
- 하지만, HTTP는 암호화되지 않는 평문 데이터를 전송하기 때문에 제 3자가 정보를 조회할 수 있다는 위험이 있다.

### HTTPS
- HTTPS (Hyper Transfer Protocol Secure)는 HTTP에 데이터 암호화가 추가되었다.
- 암호화된 데이터를 전송하기 때문에 제 3자가 볼 수 없도록 할 수 있다.
- 인터넷 상에서 정보를 암호화하는 SSL 프로토콜을 사용해 클라이언트와 서버가 자원을 주고 받을 대 쓰는 통신 규약

### HTTPS 적용
- HTTPS를 적용하기 위해서는 인증된 기관 (Certificate Authority, CA)에서 인증서를 발급받아야한다.
- CA에서 인증서를 요청하면 CA이름, 서버의 공개키, 서버의 정보를 활용하여 인증서를 생성하고 이를 CA 개인 키로 암호화하여 서버로 전송한다.
- 이때 인증서는 CA 개인 키로 암호화되니 신뢰성을 확보할 수 있다.
- 이러한 인증서를 서버측에서 발급받으면 HTTPS를 적용할 수 있다.

### HTTP 상태코드
- 200: OK 요청이 성공적으로 되었습니다.
- 201: Created 요청이 성공적이며 새로운 리소스가 생성되었습니다.
- 400: Bad Request 서버가 요청의 구문을 인식하지 못했습니다.
- 401: Unauthorized 이 요청은 인증이 필요합니다.
- 403: Forbidden 서버가 요청을 거부합니다.
- 404: Not Found 서버가 요청한 페이지를 찾을 수 없습니다.(API가 잘못되었을 때)
- 500: Internal Server Error 서버가 오류를 발생하여 요청을 수행할 수 없습니다.
