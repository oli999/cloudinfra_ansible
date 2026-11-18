# json 문서 작성법 정리

<img src="./images/image01.png">

# yml 문서와 json 문서의 차이

<img src="./images/image02.png">

# ansible playbook 실행방법

<img src="./images/image03.png">

## yml 파일의 의미

<img src="./images/image04.png">

## yml 파일에서 여러줄의 문자열 작성

<img src="./images/image05.png">

## yml 과 json 비교 1

```yml
target_packages:
  - vim
  - wget
  - curl
```

```json
{
  "target_packages": ["vim", "wget", "curl"]
}
```

## yml 과 json 비교 2

```yml
info:
  num: 1
  name: kim
  addr: seoul
```

```json
{
  "info": {
    "num": 1,
    "name": "kim",
    "addr": "seoul"
  }
}
```
## yml 과 json 비교 3

```yml
members:
  - num: 1
    name: kim
    addr: seoul
  - num: 2
    name: park
    addr: inchon
  - num: 3
    name: lee
    addr: pusan
```

```json
{
  "members": [
    {
      "num": 1,
      "name": "kim",
      "addr": "seoul"
    },
    {
      "num": 2,
      "name": "park",
      "addr": "inchon"
    },
    {
      "num": 3,
      "name": "lee",
      "addr": "pusan"
    }
  ]
}
```

## loop 테스트

<img src="./images/image06.png">