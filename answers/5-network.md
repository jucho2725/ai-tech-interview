<div align='center'>
  <h1>🌐 Network 🌐</h1>
</div>

> 질문 중 일부는 <strong>[WeareSoft님의 tech-interview](https://github.com/WeareSoft/tech-interview)</strong>를 참고하였으며, 질문에 대한 답변은 직접 작성하였습니다.

---

## Table of Contents

- [TCP/IP의 각 계층을 설명해주세요.](#1)
- [OSI 7계층와 TCP/IP 계층의 차이를 설명해주세요.](#2)
- [Frame, Packet, Segment, Datagram을 비교해주세요.](#3)
- [TCP와 UDP의 차이를 설명해주세요.](#4)
- [TCP와 UDP의 헤더를 비교해주세요.](#5)
- [TCP의 3-way-handshake와 4-way-handshake를 비교 설명해주세요.](#6)
- [TCP의 연결 설정 과정(3단계)과 연결 종료 과정(4단계)이 단계가 차이나는 이유가 무엇인가요?](#7)
- [만약 Server에서 FIN 플래그를 전송하기 전에 전송한 패킷이 Routing 지연이나 패킷 유실로 인한 재전송 등으로 인해 FIN 패킷보다 늦게 도착하는 상황이 발생하면 어떻게 될까요?](#8)
- [초기 Sequence Number인 ISN을 0부터 시작하지 않고 난수를 생성해서 설정하는 이유가 무엇인가요?](#9)
- [HTTP와 HTTPS에 대해서 설명하고 차이점에 대해 설명해주세요.](#10)
- [HTTP 요청/응답 헤더의 구조를 설명해주세요.](#11)
- [HTTP와 HTTPS 동작 과정을 비교해주세요.](#12)
- [CORS가 무엇인가요?](#13)
- [HTTP GET과 POST 메서드를 비교/설명해주세요.](#14)
- [쿠키(Cookie)와 세션(Session)을 설명해주세요.](#15)
- [DNS가 무엇인가요?](#16)
- [REST와 RESTful의 개념을 설명하고 차이를 말해주세요.](#17)
- [소켓(Socket)이 무엇인가요? 자신 있는 언어로 간단히 소켓 생성 예시를 보여주세요.](#18)
- [Socket.io와 WebSocket의 차이를 설명해주세요.](#19)
- [IPv4와 IPv6 차이를 설명해주세요.](#20)
- [MAC Address가 무엇인가요?](#21)
- [라우터와 스위치, 허브의 차이를 설명해주세요.](#22)
- [SMTP가 무엇인가요?](#23)
- [노트북으로 `www.google.com`에 접속을 했습니다. 요청을 보내고 받기까지의 과정을 자세히 설명해주세요.](#24)
- [여러 네트워크 topology에 대해 간단히 소개해주세요.](#25)
- [subnet mask에 대해서 설명해주세요.](#26)
- [data encapsulation이 무엇인가요?](#27)
- [DHCP를 설명해주세요.](#28)
- [routing protocol을 몇 가지 설명해주세요. (ex. link state, distance vector)](#29)
- [이더넷(ethernet)이 무엇인가요?](#30)
- [client와 server의 차이점을 설명해주세요.](#31)
- [delay, timing(jitter), throughput 차이를 설명해주세요.](#32)

---

## #1

#### TCP/IP의 각 계층을 설명해주세요.

#### References

---

## #2

#### OSI 7계층와 TCP/IP 계층의 차이를 설명해주세요.

#### References

---

## #3

#### Frame, Packet, Segment, Datagram을 비교해주세요.

#### References

---

## #4

#### TCP와 UDP의 차이를 설명해주세요.

#### References

---

## #5

#### TCP와 UDP의 헤더를 비교해주세요.

#### References

---

## #6

#### TCP의 3-way-handshake와 4-way-handshake를 비교 설명해주세요.

#### References

---

## #7

#### TCP의 연결 설정 과정(3단계)과 연결 종료 과정(4단계)이 단계가 차이나는 이유가 무엇인가요?

#### References

---

## #8

#### 만약 Server에서 FIN 플래그를 전송하기 전에 전송한 패킷이 Routing 지연이나 패킷 유실로 인한 재전송 등으로 인해 FIN 패킷보다 늦게 도착하는 상황이 발생하면 어떻게 될까요?

#### References

---

## #9

#### 초기 Sequence Number인 ISN을 0부터 시작하지 않고 난수를 생성해서 설정하는 이유가 무엇인가요?

#### References

---

## #10

#### HTTP와 HTTPS에 대해서 설명하고 차이점에 대해 설명해주세요.

#### References

---

## #11

#### HTTP 요청/응답 헤더의 구조를 설명해주세요.

#### References

---

## #12

#### HTTP와 HTTPS 동작 과정을 비교해주세요.

#### References

---

## #13

#### CORS가 무엇인가요?

#### References

---

## #14

#### HTTP GET과 POST 메서드를 비교/설명해주세요.

#### References

---

## #15

#### 쿠키(Cookie)와 세션(Session)을 설명해주세요.

#### References

---

## #16

#### DNS가 무엇인가요?

#### References

---

## #17

#### REST와 RESTful의 개념을 설명하고 차이를 말해주세요.

`REST`란 **Re**presentational **S**tate **T**ransfer의 약자로, <u>URI로 자원(Resource)을 명시하고 HTTP 메서드를 통해 해당 자원에 대한 CRUD 연산을 적용하는 것</u>을 의미한다.

여기서의 자원은 데이터베이스의 정보를 말한다. 하지만 클라이언트가 직접 데이터베이스에 접속해 변경하는 것은 매우 위험한 방식 이다. 그래서 이를 막기 위해 REST API를 사용하는 것이다. **클라이언트**가 서버에 데이터를 조회·생성·삭제·업데이트를 하겠다고 <u>HTTP 메서드로 요청</u>을 하면 **서버**는 로직에 따라 데이터베이스에 접근하여 <u>요청을 처리</u>한다.

`RESTful`은 REST 아키텍처로 구현된 웹 서비스를 나타내기 위한 용어로, "REST API를 제공하는 웹 서비스는 RESTful하다"처럼 사용된다.

> **HTTP 메서드 종류**

요청의 종류에 다라 다른 HTTP 메서드를 사용하는데 주로 사용하는 대표적인 메서드는 다음과 같다.

| 메서드 | 역할                                                    |
| :----: | :------------------------------------------------------ |
|  GET   | 데이터를 조회한다.                                      |
|  POST  | 데이터를 등록한다. 인증 작업을 거칠 때 사용하기도 한다. |
| DELETE | 데이터를 삭제한다.                                      |
|  PUT   | 데이터를 새 정보로 통째로 업데이트할 때 사용한다.       |
| PATCH  | 데이터의 특정 필드를 수정할 때 사용한다.                |

> **URI란?**

URI는 Uniform Resource Identifier의 약자로, 자원을 식별자로 취급하여 나타내는 주소를 말한다. URI의 종류로 URL과 URN이 있다. URI는 일반적으로 다음과 같은 형식을 갖고 있다.

<div align="center">
<img src="../images/penguin/uri.png" width="90%"/>
</div>
<br/>

#### References

- [[Network] REST란? REST API란? RESTful이란? - HeeJeong Kwon](https://gmlwjd9405.github.io/2018/09/21/rest-and-restful.html)
- [REST API 제대로 알고 사용하기 - NHN Cloud Meetup!](https://meetup.toast.com/posts/92)
- [URL과 URI의 의미와 차이점 (Difference between URL & URI) - Lael's World](https://blog.lael.be/post/61)
- [통합 자원 식별자 - 위키피디아](https://ko.wikipedia.org/wiki/%ED%86%B5%ED%95%A9_%EC%9E%90%EC%9B%90_%EC%8B%9D%EB%B3%84%EC%9E%90)
- [21장. 백엔드 프로그래밍: Node.js의 Koa 프레임워크 - 리액트를 다루는 기술](http://www.yes24.com/Product/Goods/79260300)

---

## #18

#### 소켓(Socket)이 무엇인가요? 자신 있는 언어로 간단히 소켓 생성 예시를 보여주세요.

`소켓(Socket)`이란 <u>Application 프로세스와 end-to-end 통신을 제공하는 Transport 프로토콜 사이의 인터페이스</u>을 말한다. 즉, Application에서 Transport 프로토콜을 쓰기 위한 API를 말한다.

소켓은 크게 UDP와 TCP 두종 종류로 분류할 수 있다. 자세한 내용은 [#4. TCP와 UDP의 차이를 설명해주세요.](#4)을 참고!

파이썬으로 TCP에서의 소켓과 UDP에서의 소켓 생성 코드를 구현하면 다음과 같다. 소켓을 생성한다고 바로 통신을 할 수 없으며 실제 통신을 하기 위해는 바인딩, 연결 등 추가 작업이 필요하다.

> **TCP**

- TCP Client

```python
from socket import *

server_name = "example.com"
server_port = 1234

client_socket = socket(AF_INET, SOCKET_STREAM)  # 소켓 생성
client_socket.connect((server_name, server_port)) # 서버에 연결 요청
```

- TCP Server

```python
from socket import *

server_port = 1234

server_socket = socket(AF_INET, SOCKET_STREAM)  # 소켓 생성
server_socket.bind(('', server_port)) # 소켓에 주소 바인딩
server_socket.listen(1) # 클라이언트 연결 대기

(client_socket, client_address) = server_socket.accept()  # 클라이언트 연결 수락
```

> **UDP**

- UDP Client

```python
from socket import *

server_name = "example.com"
server_port = 1234

client_socket = socket(AF_INET, SOCK_DGRAM) # 소켓 생성
```

- UDP Server

```python
from socket import *

server_port = 1234
server_socket = socket(AF_NET, SOCK_DGRAM)  # 소켓 생성
server_socket.bind(('', server_port)) # 소켓에 주소 바인딩
```

#### References

- [Chapter 2. Application Layer - Computer Networking: A Top-Down Approach](http://www.yes24.com/Product/Goods/24320296?OzSrank=2)

---

## #19

#### Socket.io와 WebSocket의 차이를 설명해주세요.

> **WebSocket**

<div align="center">
<img src="../images/penguin/web-socket.png" width="50%"/>
</div>
<br/>

`WebSocket`은 <u>서버와 브라우저 간 연결을 유지한 상태로 데이터를 교환할 수 있도록 하는 **프로토콜**</u>을 말한다.

전형적인 브라우저 렌더링 방식은 HTTP 요청에 대한 응답을 받아 브라우저 화면을 깨끗히 지우고 받은 내용을 새로 표시하는 방식인데, 내용을 지우고 다시 그리면 브라우저의 깜박임이 생기게 된다. 이러한 깜박임 없이 필요한 부분만 다시 그리는 상호작용 방식의 수요가 생겼다.

이러한 상호작용을 구현하기 위해 Pooling, Long Pooling, Streaming 등 다양한 방식을 사용했지만 요청을 보내고 응답을 보내는 **단방향 메시지 교환 규칙을 준수**하였기 때문에 상호작용하는 웹페이지를 구현하는 것은 매우 어려웠다.

이보다 쉽게 구현하기 위해 **브라우저와 서버 간 양방향 메시지 송수신 규칙**이 필요했고 이것이 WebSocket이다.

> **Socket.io**

`socket.io`는 <u>서버와 브라우저의 양방향 통신을 가능하게 하는 **모듈**</u>을 말한다. WebSocket의 경우 정말 좋은 기술이지만 오래된 브라우저의 경우 지원을 하지 않는 경우가 있다. 이런 경우 socket.io는 서버와 브라우저의 종류와 버전을 파악하여 가장 적합한 기술을 선택해 양방향 통신이 가능하도록 한다.

#### References

- [WebSocket과 Socket.io - NAVER D2](https://d2.naver.com/helloworld/1336)
- [웹소켓 - 위키백과](https://ko.wikipedia.org/wiki/%EC%9B%B9%EC%86%8C%EC%BC%93)
- [웹소켓 - 모던 JavaScript 튜토리얼](https://ko.javascript.info/websocket)
- [websocket, socket.io를 이용한 양방향 통신 - zych1751](http://www.secmem.org/blog/2019/08/17/websocket-socketio/)
- [10.5 Node.js(Express)와 Socket.io - PoiemaWeb](https://poiemaweb.com/nodejs-socketio)

---

## #20

#### IPv4와 IPv6 차이를 설명해주세요.

IPv4와 IPv6는 **인터넷 프로토콜(IP)의 버전**을 말하며, IPv4는 IP의 4번째 버전, IPv6는 IP의 6번째 버전을 말한다. 이 때 인터넷 프로토콜은 호스트 간 패킷 교환 네트워크에서 패킷(Packet) 혹은 데이터그램(Datagram)으로 불리는 정보를 주고받는데 사용하는 프로토콜을 말한다.

<div align="center">
<img src="../images/penguin/ipv4-ipv6.png" width="80%"/>
</div>
<br/>

`IPv4`는 헤더에 options이 존재하고, fragmentation/reassembly 기능을 제공해 MTU(Maximum Transport Unit)을 넘는 큰 데이터그램을 쪼개 전송을 하고 도착지에서 재조합을 한다. 또한 checksum 비트도 존재하여 매 라우터마다 checksum 비트를 갱신한다.

반면 `IPv6`는 빠른 속도를 위해 fragmentation/reassembly 기능을 제공하지 않으며, 데이터그램의 우선순위를 설정할 수 있는 priority 비트가 존재한다.

#### References

- [Chapter 4. Network Layer - Computer Networking: A Top-Down Approach](http://www.yes24.com/Product/Goods/24320296?OzSrank=2)

---

## #21

#### MAC Address가 무엇인가요?

`MAC 주소(Media Access Control Address)`는 Data Link Layer에서 통신을 위해 **네트워크 인터페이스에 할당한 식별자**를 말한다. 즉, 모든 네트워크 장비는 자신의 MAC 주소가 있으며 주소는 장비 제조업체가 할당한다. MAC 주소는 물리적 주소(Physical Address)라고 불리기도 한다.

#### References

- [MAC 주소 - 위키백과](https://ko.wikipedia.org/wiki/MAC_%EC%A3%BC%EC%86%8C)

---

## #22

#### 라우터와 스위치, 허브의 차이를 설명해주세요.

> 여기서의 네트워크는 LAN(Local Area Network)를 말합니다.

`라우터(Router)`는 **네트워크 사이를 연결하는 장치**로, 최종 도착지의 네트워크에 도착할 수 있도록 적절한 경로를 설정하여 패킷을 전송한다.

`스위치(Switch)`는 **네트워크 내에서 패킷을 전송하는 장치**를 말한다. 스위치로 요청이 들어오면 IP 주소에 대응되는 MAC 주소를 찾아 해당 MAC 주소로 패킷을 전송한다. 만약 IP 주소에 대응되는 MAC 주소가 없다면 허브처럼 브로드캐스트 방식으로 패킷을 전송하고 IP 주소와 MAC 주소를 대응시킨 테이블을 갱신시킨다.

`허브(Hub)`는 **여러 기기를 연결하여 네트워크를 만들어주는 장치**로, 패킷을 받으면 연결된 모든 기기에 패킷을 전송한다.

#### References

- [허브, 라우터, 공유기, 스위치의 개념과 차이점 - Easy is Perfect](http://melonicedlatte.com/network/2019/12/21/154500.html)
- [네트워크 스위치와 허브, 라우터는 어떻게 다른 걸까 - IT WORLD](https://www.itworld.co.kr/news/167585)
- [라우터 그리고 스위치 - HelloWorld](https://server-engineer.tistory.com/582)

---

## #23

#### SMTP가 무엇인가요?

`SMTP(Simple Mail Transfer Protocol)`은 **인터넷에서 이메일을 보내기 위해 사용하는 TCP/IP 프로토콜**을 말한다. 사용하는 TCP Port 번호는 25번이다.

SMTP는 다음의 명령어를 사용하여 메일을 주고 받는다.

- MAIL 명령: 주소 반환 확립
- RCPT 명령: 메시지 수신자 확립
- DATA 명령: 메시지 텍스트의 첫 신호를 제공

#### References

- [간이 우편 전송 프로토콜 - 위키백과](https://ko.wikipedia.org/wiki/%EA%B0%84%EC%9D%B4_%EC%9A%B0%ED%8E%B8_%EC%A0%84%EC%86%A1_%ED%94%84%EB%A1%9C%ED%86%A0%EC%BD%9C)

---

## #24

#### 노트북으로 `www.google.com`에 접속을 했습니다. 요청을 보내고 받기까지의 과정을 자세히 설명해주세요.

> **1단계**

웹 사이트에 접속하기 위해서는 **노트북의 IP주소, 1-hop 라우터의 IP 주소, DNS 서버 주소**가 필요하다. 이를 알아 내기 위해 DHCP query가 담긴 IP 데이터그램을 1-hop 라우터에게 전송한다. DHCP 서버가 내장된 라우터가 노트북의 IP주소, 자신의 IP주소, DNS 서버의 IP주소를 답은 DHCP ACK를 다시 노트북에게 전송한다.

- DNS란 **D**omain **N**ame **S**ystem의 약자로 `www.google.com`과 같은 도메인 주소를 IP 주소로 바꿔주는 시스템을 말한다.
- DHCP 서버는 보통은 라우터에 DHCP 서버가 내장되어 있으며 DHCP 서버에 연결된 클라이언트에게 자동적으로 IP주소를 할당한다.

> **2단계**

DNS 서버에 DNS query를 보내기 전에 **1-hop 라우터의 MAC 주소**가 필요하므로 ARP query를 브로드캐스트 방식으로 전송하여 router의 MAC주소를 알아낸다.

- ARP란 **A**ddress **R**esolution **P**rotocol의 약자로, MAC 주소와 IP 주소를 1:1 매핑하기 위해 사용된다.

> **3단계**

`www.google.com`에 요청을 보내기 위해서는 `www.google.com`의 IP주소가 필요하므로, DNS query가 담긴 IP 데이터그램을 DNS 서버에 전송하고 `www.google.com`의 IP 주소를 클라이언트인 노트북에게 전송한다.

> **4단계**

TCP 소켓을 생성하고 3-way handshake로 연결을 생성한다. HTTP 요청을 보내고 응답을 받아 브라우저에 렌더링을 하면 Google 웹페이지를 브라우저에서 확인할 수 있다.

#### References

- [Chapter 6.7. Life of a web request - Computer Networking: A Top-Down Approach](http://www.yes24.com/Product/Goods/24320296?OzSrank=2)
- [ARP 쉽게 이해하기 - 네트워크 엔지니어 환영의 AWS 기술블로그](https://aws-hyoh.tistory.com/entry/ARP-%EC%89%BD%EA%B2%8C-%EC%9D%B4%ED%95%B4%ED%95%98%EA%B8%B0)

---

## #25

#### 여러 네트워크 topology에 대해 간단히 소개해주세요.

#### References

---

## #26

#### subnet mask에 대해서 설명해주세요.

#### References

---

## #27

#### data encapsulation이 무엇인가요?

#### References

---

## #28

#### DHCP를 설명해주세요.

#### References

---

## #29

#### routing protocol을 몇 가지 설명해주세요. (ex. link state, distance vector)

#### References

---

## #30

#### 이더넷(ethernet)이 무엇인가요?

#### References

---

## #31

#### client와 server의 차이점을 설명해주세요.

#### References

---

## #32

#### delay, timing(jitter), throughput 차이를 설명해주세요.

#### References

---

```

```