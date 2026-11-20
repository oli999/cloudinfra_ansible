## amazon linux ec2 만들기

<img src="./images/image01.png">
<img src="./images/image02.png">
<img src="./images/image03.png">
<img src="./images/image04.png">
<img src="./images/image05.png">


## 테스트로 ec2 에 접속해 보기

```bash
chmod 600 ~/.ssh/ec2-key.pem
ssh ec2-user@43.201.113.81 -i ~/.ssh/ec2-key.pem
```
<img src="./images/image06.png">
<img src="./images/image07.png">
<img src="./images/image08.png">


## ec2_bootstrap.yml 을 실행해서 user1 을 만들고 접속 가능한지 확인

```bash
ansible-playbook ec2_bootstrap.yml
ssh user1@43.201.113.81 -i ~/.ssh/ansiblekey.pem
```
<img src="./images/image10.png">

## fastapi_setup.yml 파일을 ansible 로 실행후에 접속해서 확인해 본다

```bash
# mgmt 에서 실행
ansible-playbook fastapi_setup.yml
ssh user1@43.201.113.81 -i ~/.ssh/ansiblekey.pem

# 접속된 이후니까 ec2 에서 실행 
curl localhost:8000
curl localhost:8001
```

## 웹브라우저로 ec2 의 public ip 로 접속 테스트

<img src="./images/image11.png">
<img src="./images/image12.png">
<img src="./images/image13.png">
<img src="./images/image14.png">
<img src="./images/image15.png">

