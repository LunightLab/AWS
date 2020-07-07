<div align=right>
    <a href="https://github.com/LunightLab">
        <img alt="author" src= "https://img.shields.io/badge/author-lunight-blue?style=glat-square" target="_blank"></a>
    </a>
    <a href="https://github.com/LunightLab/LuLabTemplate">
        <img alt="template version" src= "https://img.shields.io/badge/template%20version-1.0-blue?style=glat-square" target="_blank"></a>
    </a>
</div>

AWS-Cloud Practitioner Essentials(Second-Edition)
=================================================

**<div align=right>AWS의 통합형 서비스</div>**

### Application Load Balancer

<p align="center"><img src="./img/ALB-lb1.png" width="600" height="300"></p>  

**ALB**  
- ALB(Application Load Balancer)는 Elastic Load Balancing 서비스의 일부로 도입된 두번째 유형으 로드밸런서이다.  
- Classic Load Balancer가 제공하는 대부분의 기능을 제공하고 추가로 중요한 기능과 개선사항이 추가되었다.

<p align="center"><img src="./img/ALB-lb2.png" width="600" height="300"></p>   

**향상된 기능**  
- 지원하는 프로토콜 : HTTP, HTTPS, HTTP/2, WebSockets  
- CloudWatch 지표 : 추가적인 로드밸런싱 지표 및 대상 그룹 지표 차원  
- Access Log : WebSocket 연결의 세부정보를 볼 수 있는 기능  
- Status check : 더욱 세분화된 수준에서 대상 및 애플리케이션 상태에 대한 통찰력

**기타 기능**  
- 경로 및 호스트 기반 라우팅 : 경로 기반으로 요청을 각기 다른 대상 그룹으로 전달하는 규칙을 제공. 호스트 기반은 호스트 이름에 따라 요청을 각 다른 대상 그룹으로 전달하는 규칙을 정의하는데 사용할 수 있다.  
- 네이티브 IPV6 지원  
- 삭제 보호 및 요청 추적 : 요청 추적은 클라이언트에서 대상으로 http요청을 추적하는데 사용할 수 있다.  
- 동적 포트 : AmazonECS는 Application Load Balancer와 통합되어 일정이 예약된 컨테이너에서 사용하는 동적 포트를 노출한다.  
- AWS WAF

**주요용어**  
- 리스너 : 리스너는 구성한 프로토콜 및 포트를 사용하여 연결 요청을 확인하는 프로세스이다. 리스너에 대해 정의한 규칙에 따라 로드 밸런서가 하나 이상의 대상 그룹에 있는 목적지로 라우팅 하는 방법이 결정된다.  
- 대상 : 설정된 리스너 규칙에 때른 트래픽 목적지이다.  
- 대상 그룹 : 각 대상 그룹은 지정된 프로토콜과 포트 번호를 사용하여 하나 이상의 등록된 대상으로 요청을 라우팅한다. 상태 확인은 대상 그룹별로 구성될 수 있다.

### Auto Scaling

<p align="center"><img src="./img/AutoScaling-4.png" width="500" height="300"></p>   

-	Auto Scling을 사용하면 애플리케이션 로드를 처리할 수 있는 적절한 수의 EC2 인스턴스를 유지하여 리소스를 최소화할 수 있다.  
-	워크로드 요구 사항을 충족하기 위해 필요한 시점에 EC2 인스턴스 수를 추측할 필요가 없다.  
-	Auto Scling을 사용하면 지정한 조건에 따라 EC2 인스턴스를 추가하거나 제거할 수 있다.  
-	Auto Scling은 성능 요구 사항이 변화하는 환경에서 강력하다. 이를 통해 성능을 유지하고 비용을 최소화하여 운영할 수 있다.  

**질의**

<p align="center"><img src="./img/AutoScaling-2.png" width="700" height="280"></p>  

Q. 내 워크로드에 변화하는 성능 요구사항을 충족하기 위해 충분한 EC2 리소스가 있는지 어떻게 확인 할 수 있는가?  
A. 확장성  
Q. 온디맨드로 EC2 리소스 프로비저닝을 자동화할 수 있는가?  
A. 자동화

**WatchCloud**

<p align="center"><img src="./img/AutoScaling-1.png" width="700" height="350"></p>   

EC2 인스턴스에서 애플리케이션을 실행할 때 Amazon CloudWatch를 이용하여 워크로드 성능을 모니터링하는것이 중요하다. CloudWatch 자체에서 인스턴스를 추가하거나 제거하지 않기 때문에 **AutoScaling**이 필요함

**자동으로 확장하기 위한 AutoScaling의 필수 3가지 구성요소**  
<p align="center"><img src="./img/AutoScaling-3.png" width="600" height="300"></p>

-	시작 구성 생성(What?)

	-	사용할 AMI(Amazon Machine Image)  
	-	인스턴스에 적용할 인스턴스 유형  
	-	보안 그룹  
	-	역할  

-	AutoScling 그룹 생성(Where?)

	-	로드 밸런서와 상호 작용할 인스턴스를 배포할 VPC와 서브넷 정의  
	-	그룹에 대한 경계를 지정(최소-최대 인스턴스 및 용량)  

-	하나 이상의 Auto Scling 정책 정의(When?)

	-	예약  
	-	확장 또는 축소 시간을 정의  
	-	온디맨드  
	-	조건 기반 정책은 Auto Scling을 동적으로 만들어 변화하는 요구사항을 충족할 수 있다.  

### Amazon Route 53

준비중...

### Amazon Relational Database Services(RDS)

준비중...

### AWS Lamda

준비중...

### AWS Elastic Beantalk

준비중...

### Amazon Simple Notification Service(SNS)

준비중...

### Amazon CloutWatch

준비중...

### Amazon CloudFront

준비중...

### AWS CloutFormation

준비중...

<div align="center">

<sub><sup>Written by <a href="https://github.com/LunightLab">@Lunight</a></sup></sub><small></small>

</div>
