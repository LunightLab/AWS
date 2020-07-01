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

**<div align=right>AWS의 핵심서비스</div>**

### Amazon EC2(Elastic Cloud Compute)

-	**Compute** : 표시되고 있는 컴퓨팅 또는 **서버 리소스를 나타내며 서버를 활용하여 여러 활동을 할 수 있다.**  
-	**Cloud** : 클라우드에서 호스팅 되는 컴퓨팅 리소스  
-	**Elastic(탄력적)** : 애플리케이션의 현 요구사항에 따라 해당 **애플리케이션에 필요한 리소스를 자동으로 늘리거나 줄일 수 있음**  
-	서버라는 이름 대신 **Amazon EC2 인스턴스라는 용어를 사용**  
-	인스턴스는 사용량에 따라 요금을 지불(인스턴스를 실행하는 시간을 측정)  
-	광범위한 하드웨어와 소프트웨어가 제공되고 인스턴스를 호스트 할 위치를 선택할 수 있다.  

### Amazon EBS(Elastic Block Storage)

-	EBS 볼륨은 Amazon EC2 인스턴스의 스토리지 단위로 사용할 수 있다.  
-	AWS에서 실행 중인 인스턴스의 디스크 공간이 필요할 때마다 EBS 볼륨을 기억  
-	볼륨은 HDD 또는 SSD가 될 수 있다.  
-	사용한 만큼 지불할 수 있고, 볼륨이 더이상 필요하지 않을 때마다 이를 삭제하여 요금을 지불하지 않을 수 있다.  
-	EBS 볼륨은 **안정성과 가용성을 목표로 설계됨.** 볼륨에 있는 데이터는 자동으로 가용 영역(AZ)에서 실행중인 여러 서버에 복제된다.  

### Amazon S3(Simple Storage Service)

-	**Amazon S3는 데이터를 저장하고 검색할 수 있는 간단한 API를 제공하는 완전 관리형 스토리지 서비스**  
-	Amazon S3 객체는 원하는 만큼 추가할 수 있다.  
-	객체는 이미지, 동영상 또는 서버 로그와 같은 거의 모든 데이터 파일이 될 수 있으며, 최대 몇 테라바이트 크기의 객체를 지원하므로, 데이터베이스 **스냅샷** 을 객체로 저장할 수도 있다.  
-	Amazon S3는 http또는 https를 통해 인터넷에서 데이터에 대한 지연 시간이 짧은 액세스를 제공하므로 언제 어디서나 데이터를 검색할 수 있다.  
-	VPC 종단점을 통해 S3에 private access할 수 있다.  

<!--
### AWS 클라우드

-   AWS를 통해 서버, 데이터베이스, 스토리지 및 상위 애플리케이션 구성요소를 몇 초 이내에 엑세스 할 수 있다.
-   임시 또는 일회용 리소스로 취급할 수 있어 고정적이고 유한한 IT인프라를 경직성과 제약으로부터 자유로울 수 있다.  

### AWS 클라우드 특성

#### 민첩성 (Agility)

-   **속도(Speed)** : 막대한 투자와 비용이 필요없이 전세계 네트워크에 빠르게 서비스가 가능  
-   **실험(Experimentation)** : 클라우드 환경을 통해 실험을 자주 할 수 있으며 빈번한 실험을 통해 새로운 구성과 탐색이 가능하다.  
-   **혁신의 문화 (Culture of innovation)**  
-   **CloudFormation** 을 통해 일관적이고 템플릿화된 개발 환경 구축이 가능하다.  
    *CloudFormation - AWS에서 제공하는 템플릿이나 개발자 혹은 시스템 관리자가 작성한 템플릿을 이용해 AWS 리소스들을 쉽게 생성하고 관리하는 방법을 제공한다.*

#### 내결함성

-   시스템 구성 요소에 장애가 발생하더라도 시스템이 작동 가능 상태를 유지하는 능력(애플리케이션 구성 요소의 기본적인 중복성)

#### 고가용성

-   사용자 개입 없이 시스템이 항상 자동으로 액세스 가능하며 가동 중지가 최소화되도록 하는 능력

### 탄력성

-   간편하게 컴퓨팅 리소스의 규모를 확장하거나 축소할 수 있는 능력  
-->

<div align="center">

<sub><sup>Written by <a href="https://github.com/LunightLab">@Lunight</a></sup></sub><small></small>

</div>
