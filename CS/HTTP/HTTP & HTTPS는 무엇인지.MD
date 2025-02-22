a#### <인터넷 PART 목차>

> - ~~인터넷은 어떻게 작동하는지~~

- **HTTP & HTTPS는 무엇인지**
- 브라우저 동작원리
- DNS와 작동원리
- 도메인 네임은 무엇인지
- 호스팅은 무엇인지

### \*🔐Study Keyword :

> ✅ HTTP와 HTTPS는 무엇이고 어떤 차이가 있을까?

# HTTP

**WHAT IS❓**

#### - HTTP(HyperText Transfer Protocol)

> - **HTTP란**? 인터넷 상의 커뮤니케이션에 사용되는 형식들을 중 하나로 *인터넷 상에서 클라이언트와 서버가 자원을 주고 받을 때 쓰는 통신 규약*에 의미를 지닌다.

- HTTP는 텍스트 교환이므로, 누군가 네트워크에서 신호를 가로채면 내용이 노출되는 보안 이슈가 존재한다.

#### - http/https 활용 예시

> 1> 유저의 컴퓨터에서 네이버 서버에 요청을 보낼 때 마다 '메시지들이 http 혹은 https 형식인지' 주소 창에 써서 일일이 명시해줘야한다.
> 2> 명시해주었다면 네이버 서버는 그에 맞는 형식으로 읽어본 다음 어떠한 폐이지를 보여달라는 건지 요청을 인지하여 그에 맞는 응답을 작성해서 보낸다.
> 3> 이후 유저의 컴퓨터에서 그것을 http 혹은 https 형식에 따라 해독해서 네이버 화면을 보여주게 된다.
> 4> http 형식에 **보안** 기능까지 추가하여 보안문제를 해결한 프로토콜이 바로 **HTTPS이다**.

# HTTPS

#### HTTPS(HyperText Transfer Protocol _Secure_)

> - **HTTPS란**? *인터넷 상에서 정보를 암호화하는 SSL 프로토콜*을 사용해 _클라이언트와 서버가 자원을 주고 받을 때 쓰는 통신 규약_

- HTTPS는 텍스트를 암호화한다. (공개키 암호화 방식으로)

### HTTP VS HTTPS

#### HTTPS는 그렇다면 보안 문제를 무엇으로부터 보호해줄까?

#### 1. HTTPS는 유저가 어떤 웹 사이트로부터 보내는 정보를 다른 누군가가 훔쳐보지 못하게 한다.

EX> 네이버에 접속해서 아이디와 비밀번호를 입력하는 경우 로그인 버튼을 누르면 ID, PSW 전부가 인터넷을 타고 네이버에 서버로 전송된다.

> ![](https://images.velog.io/images/minj9_6/post/6370e462-d96b-4be9-a5e2-ee5c1b2869cd/image.png)
> 1> **http**로 보내면 이 암호가 입력한 텍스트 그대로 누구나 알아볼 수 있는 형식으로 보내지기 때문에 누군가가 이 정보를 중간에 들여다 보면 유저의 ID, PSW를 알 수 있게된다.

> ![](https://images.velog.io/images/minj9_6/post/4d320d60-b38f-4945-9828-4b46c8b695d7/image.png)
> 2> **https**는 이 정보를 네이버만 알아볼 수 있는 뒤죽박죽이 된 텍스트로 변경하여 실어 보내기 때문에 누군가 들여다봐도 뭐라고 쓴건지 알아볼 수 없다.

#### 2. 유저가 접속한 사이트가 신뢰 할 수 있는 사이트 인지를 판별해 준다.

EX> 네이버가 아닌 네이놈이라는 피싱 사이트에 유조가 접속해 ID, PSW를 입력하면 피싱사이트에서 유저의 정보를 알게된다.

> 1> **https는** 이러한 수상한 사이트를 걸러내준다. 왜냐하면 기관으로부터 검증된 사이트만 주소에 https 사용이 허가되기 때문이다
> 2> 반연 **http를** 사용한 사이트들은 주소창에 Not Secure과 같은 표시가 뜨게된다.

### \*💡conclusion

>

- HTTP와 HTTPS는 모두 **하이퍼 텍스트 문서 전송 프로토콜**이지만 HTTPS는 중요한 데이터, 정보 및 파일을 클라이언트에서 서버로, 그리고 그 반대로 인터넷에서 **안전하게 전송할 수있는 안전한 방법**을 제공합니다.

### #📑Study Source

> - https://ko.gadget-info.com/difference-between-http, HTTP와 HTTPS의 차이점

- https://www.youtube.com/watch?v=H6lpFRpyl14&t=65s, 얄코 HTTPS가 뭐고 왜 쓰나요? (Feat. 대칭키 vs. 비대칭키)
- https://gyoogle.dev/blog/computer-science/network/HTTP%20&%20HTTPS.html

#### <인터넷 PART 목차>

> - ~~인터넷은 어떻게 작동하는지~~

- **HTTP & HTTPS는 무엇인지**
- 브라우저 동작원리
- DNS와 작동원리
- 도메인 네임은 무엇인지
- 호스팅은 무엇인지

### \*🔐Study Keyword :

> ✅ HTTP와 HTTPS는 무엇이고 어떤 차이가 있을까?

# HTTP

**WHAT IS❓**

#### - HTTP(HyperText Transfer Protocol)

> - **HTTP란**? 인터넷 상의 커뮤니케이션에 사용되는 형식들을 중 하나로 *인터넷 상에서 클라이언트와 서버가 자원을 주고 받을 때 쓰는 통신 규약*에 의미를 지닌다.

- HTTP는 텍스트 교환이므로, 누군가 네트워크에서 신호를 가로채면 내용이 노출되는 보안 이슈가 존재한다.

#### - http/https 활용 예시

> 1> 유저의 컴퓨터에서 네이버 서버에 요청을 보낼 때 마다 '메시지들이 http 혹은 https 형식인지' 주소 창에 써서 일일이 명시해줘야한다.
> 2> 명시해주었다면 네이버 서버는 그에 맞는 형식으로 읽어본 다음 어떠한 폐이지를 보여달라는 건지 요청을 인지하여 그에 맞는 응답을 작성해서 보낸다.
> 3> 이후 유저의 컴퓨터에서 그것을 http 혹은 https 형식에 따라 해독해서 네이버 화면을 보여주게 된다.
> 4> http 형식에 **보안** 기능까지 추가하여 보안문제를 해결한 프로토콜이 바로 **HTTPS이다**.

# HTTPS

#### HTTPS(HyperText Transfer Protocol _Secure_)

> - **HTTPS란**? *인터넷 상에서 정보를 암호화하는 SSL 프로토콜*을 사용해 _클라이언트와 서버가 자원을 주고 받을 때 쓰는 통신 규약_

- HTTPS는 텍스트를 암호화한다. (공개키 암호화 방식으로)

### HTTP VS HTTPS

#### HTTPS는 그렇다면 보안 문제를 무엇으로부터 보호해줄까?

#### 1. HTTPS는 유저가 어떤 웹 사이트로부터 보내는 정보를 다른 누군가가 훔쳐보지 못하게 한다.

EX> 네이버에 접속해서 아이디와 비밀번호를 입력하는 경우 로그인 버튼을 누르면 ID, PSW 전부가 인터넷을 타고 네이버에 서버로 전송된다.

> ![](https://images.velog.io/images/minj9_6/post/6370e462-d96b-4be9-a5e2-ee5c1b2869cd/image.png)
> 1> **http**로 보내면 이 암호가 입력한 텍스트 그대로 누구나 알아볼 수 있는 형식으로 보내지기 때문에 누군가가 이 정보를 중간에 들여다 보면 유저의 ID, PSW를 알 수 있게된다.

> ![](https://images.velog.io/images/minj9_6/post/4d320d60-b38f-4945-9828-4b46c8b695d7/image.png)
> 2> **https**는 이 정보를 네이버만 알아볼 수 있는 뒤죽박죽이 된 텍스트로 변경하여 실어 보내기 때문에 누군가 들여다봐도 뭐라고 쓴건지 알아볼 수 없다.

#### 2. 유저가 접속한 사이트가 신뢰 할 수 있는 사이트 인지를 판별해 준다.

EX> 네이버가 아닌 네이놈이라는 피싱 사이트에 유조가 접속해 ID, PSW를 입력하면 피싱사이트에서 유저의 정보를 알게된다.

> 1> **https는** 이러한 수상한 사이트를 걸러내준다. 왜냐하면 기관으로부터 검증된 사이트만 주소에 https 사용이 허가되기 때문이다
> 2> 반연 **http를** 사용한 사이트들은 주소창에 Not Secure과 같은 표시가 뜨게된다.

### \*💡conclusion

>

- HTTP와 HTTPS는 모두 **하이퍼 텍스트 문서 전송 프로토콜**이지만 HTTPS는 중요한 데이터, 정보 및 파일을 클라이언트에서 서버로, 그리고 그 반대로 인터넷에서 **안전하게 전송할 수있는 안전한 방법**을 제공합니다.

### #📑Study Source

> - https://ko.gadget-info.com/difference-between-http, HTTP와 HTTPS의 차이점

- https://www.youtube.com/watch?v=H6lpFRpyl14&t=65s, 얄코 HTTPS가 뭐고 왜 쓰나요? (Feat. 대칭키 vs. 비대칭키)
- https://gyoogle.dev/blog/computer-science/network/HTTP%20&%20HTTPS.html
