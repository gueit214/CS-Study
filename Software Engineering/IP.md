## IP

### IP(Internet Protocol)

- 인터넷에 연결되어 있는 모든 장치들을 식별할 수 있도록 각각에 부여되는 고유 주소이다.
- 네트워크 데이터가 각 장치에 도달하기 위해 주소 정보가 필요한다.

## IP 종류

### IPv4

![image](https://github.com/kknyapple/CS-Study/assets/72698829/1ce474da-6ff9-4caf-8af4-1bf3ca112965)


- 현재 대부분 쓰이는 IP 주소이다.
- 10진법으로 마침표로 구분된 4개의 숫자로 쓰이고, 2진법으로는 32비트 숫자로 표현 된다.
- 약 43억개(2^32)의 주소를 가진다.
- 사설 IP와 같은 개념으로 IPv4가 부족하지만 지금까지 문제 없이 사용되고 있다.

### IPv6

![image](https://github.com/kknyapple/CS-Study/assets/72698829/bf567e67-dafd-482a-8cdc-c1da8b1d8567)


- IPv4 주소 고갈 문제로 IPv6가 등장했다.
- 128비트로 표현된다.
- 네트워크 속도, 보안적인 부분에서 IPv4 보다 뛰어나다.
- 기준 주소체계를 변경하는데 비용이 많이 들어 완전히 상용화되지 못했다.

## 공인 IP/사설 IP/고정 IP/유동 IP

### 고정 IP

- 컴퓨터에 고정적으로 부여된 IP이다.
- 한 번 부여되면 다른 장비에 부여할 수 없어 보안성이 우수하다.

### 유동 IP

- 대부분의 사용자가 사용한다.
- 유동적인 IP로 인터넷 사용자 모두에게 고정 IP를 부여해 주기 힘들기 때문에 사용된다.
- 사용자들이 인터넷에 접속하는 매 순간마다 사용하고 있지 않는 IP 주소를 발급해 준다.

### 공인 IP

- IP 주소는 임의로 부여하는 것이 아니라 전 세계적으로 ICANN이라는 기관이 국가 별로 사용할 IP 대역을 관리한다.
- 우리나라는 한국인터넷진흥원(KISA)에서 국내 IP 주소들을 관리한다.
- 국내 IP 주소를 ISP(Internet Service Provider: KT, LG, SKT 통신사)가 부여받고 이 IP를 제공 받아 인터넷을 사용한다.
- 이렇게 발급 받은 IP를 공인 IP라 한다.

### 사설 IP

- 공유기로 인터넷을 사용할 때 공유기까지는 공인 IP를 할당하지만 공유기에 연결되어 있는 각 네트워크 기기는 사설 IP를 할당한다.
- 사설 IP는 어떤 네트워크 안에서만 내부적으로 사용되는 고유한 주소로, 하나의 네트워크 안에서 유일하다.
- 같은 대역의 사설 IP에 있지 않은 경우 접속이 불가하다.

## NAT

### 사설망

- 사설 IP를 할당해 그룹으로 묶는 방법이다.
- 번호는 같더라도 네트워크가 다르면 전혀 다른 목적지 주소를 나타낼 수 있다. (한 네트워크 내에서는 중복되지 않고 식별되어야 한다.)

### NAT

![image](https://github.com/kknyapple/CS-Study/assets/72698829/bed52f48-32f2-4ddb-87c0-d1177f49742e)

- 외부 인터넷 입장에서 주소 번호가 똑같은 사설 IP들을 구분해야한다.
- NAT(Network Adress Translation) 변환으로 인터넷 주소 변역 기능을 사용한다.
- 공유기에 연결되어 있는 컴퓨터들의 사설 IP를 받아와 공인 IP로 변환한 후 외부 인터넷으로 공인 IP 주소 정보를 보낸다.

### 참고
- https://inpa.tistory.com/entry/JS-%F0%9F%93%9A-%EB%B9%84%EB%8F%99%EA%B8%B0%EC%B2%98%EB%A6%AC-async-await#async_/_await_%EA%B8%B0%EB%B3%B8_%EC%82%AC%EC%9A%A9%EB%B2%95