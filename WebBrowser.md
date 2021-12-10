# 웹 브라우저

웹은 인터넷이라는 글로벌 네트워크 위에 구현되어 있음. 정해진 프로토콜을 기반으로 통신함.

웹 브라우저는 뛰어난 이용자 경험(User Experience, UX)을 제공하는 소프트웨어 중 하나임. 이용자는 브라우저를 이용하여 쉽게 정보를 검색하고, 동영상을 보고, 파일을 내려받지만 내부에서 어떠한 연산이 일어나는지는 전혀 알지 못함.

# URL

URL은 Uniform Resource Locator의 약자로, 웹에 있는 리소스의 위치를 표현하는 문자열임. 브라우저로 특정 웹 리소스에 접근할 때는, URL을 사용하여 이를 서버에게 요청함.

URL은 Scheme, Authority (Userinfo, Host, Port), Path, Query, Fragment 등으로 구성됨.

Scheme: 웹 서버와 어떤 프로토콜로 통신할지 나타냄.

Host: Authority의 일부로, 접속할 웹 서버의 주소에 대한 정보를 가지고 있음.

Port: Authority의 일부로, 접속할 웹 서버의 포트에 대한 정보를 가지고 있음.

Path: 접근할 웹 서버의 리소스 경로로 '/'로 구분됨.

Query: 웹 서버에 전달하는 파라미터이며 URL에서 '?' 뒤에 위치함.

Fragment: 메인 리소스에 존재하는 서브 리소스를 접근할 때 이를 식별하기 위한 정보를 담고 있음. '#' 문자 뒤에 위치함.

### [Http://example.com/path?search=1#fragment](Http://example.com/path?search=1#fragment)

Scheme | http:// | 웹 브라우저가 어떤 통신 규약(프로토콜)을 사용할지 지정함. 보통 http/https를 사용함.

Host | [example.com](http://example.com) | 웹 브라우저가 어디에 연결할지 정하는 호스트 주소임. 도메인이나 IP Addrest가 호스트로써 사용될 수 있음.

Path | /path | 웹 브라우저가 연결하려고 하는 리소스에 대한 경로임.

Query | ?search=1 | 웹 브라우저가 서버에게 전달하는 파라미터임.

Fragment | #fragment | 웹 브라우저만 가지고 있는 데이터임. 메인 리소스 (페이지) 내에서 서브 리소스를 식별할 때 사용함.

# Domain Name

URL 구성 요소 중 Host는 웹 브라우저가 접속할 웹 서버의 주소를 나타냄. Host는 Domain Name, IP Address의 값을 가질 수 있음.

IP Address는 네트워크 상에서 통신이 이루어질 때 장치를 식별하기 위해 사용되는 주소임.

불규칙한 숫자로 이루어진 IP Address는 사람이 외우기 어려우므로, 일반적으로는 도메인의 특성을 담은 이름을 정의하여 IP 대신 사용함.

Domain Name을 Host 값으로 이용할 때, 브라우저는 Domain Name Server(DNS)에 Domain Name을 질의하고, DNS가 응답한 IP Address를 사용함.