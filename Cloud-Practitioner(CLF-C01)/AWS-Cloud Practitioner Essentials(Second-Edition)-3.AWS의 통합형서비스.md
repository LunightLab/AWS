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

<!--
### Amazon EC2(Elastic Cloud Compute)

-   **Compute** : 표시되고 있는 컴퓨팅 또는 **서버 리소스를 나타내며 서버를 활용하여 여러 활동을 할 수 있다.**  
-   **Cloud** : 클라우드에서 호스팅 되는 컴퓨팅 리소스  
-   **Elastic(탄력적)** : 애플리케이션의 현 요구사항에 따라 해당 **애플리케이션에 필요한 리소스를 자동으로 늘리거나 줄일 수 있음**  
-   서버라는 이름 대신 **Amazon EC2 인스턴스라는 용어를 사용**  
-   인스턴스는 사용량에 따라 요금을 지불(인스턴스를 실행하는 시간을 측정)  
-   광범위한 하드웨어와 소프트웨어가 제공되고 인스턴스를 호스트 할 위치를 선택할 수 있다.  

### Amazon EBS(Elastic Block Storage)

-   EBS 볼륨은 Amazon EC2 인스턴스의 스토리지 단위로 사용할 수 있다.  
-   AWS에서 실행 중인 인스턴스의 디스크 공간이 필요할 때마다 EBS 볼륨을 기억  
-   볼륨은 HDD 또는 SSD가 될 수 있다.  
-   사용한 만큼 지불할 수 있고, 볼륨이 더이상 필요하지 않을 때마다 이를 삭제하여 요금을 지불하지 않을 수 있다.  
-   EBS 볼륨은 **안정성과 가용성을 목표로 설계됨.** 볼륨에 있는 데이터는 자동으로 가용 영역(AZ)에서 실행중인 여러 서버에 복제된다.  

### Amazon S3(Simple Storage Service)

-   **Amazon S3는 데이터를 저장하고 검색할 수 있는 간단한 API를 제공하는 완전 관리형 스토리지 서비스**  
-   Amazon S3 객체는 원하는 만큼 추가할 수 있다.  
-   객체는 이미지, 동영상 또는 서버 로그와 같은 거의 모든 데이터 파일이 될 수 있으며, 최대 몇 테라바이트 크기의 객체를 지원하므로, 데이터베이스 **스냅샷** 을 객체로 저장할 수도 있다.  
-   Amazon S3는 http또는 https를 통해 인터넷에서 데이터에 대한 지연 시간이 짧은 액세스를 제공하므로 언제 어디서나 데이터를 검색할 수 있다.  
-   VPC 종단점을 통해 S3에 private access할 수 있다.  

### AWS Global Infrastructure

-   AWS의 글로벌 인프라를 Resion, AZ, Edge location으로 나뉜다.  

#### 리전

-   2개 이상의 가용 영역을 호스팅 하는 지리적 영역이다.  
-   AWS 서비스에 대한 구성 수준.  
-   AWS를 사용해 리소스를 배포할 때 리소스가 위치하는 리전을 선택한다.  
-   비용을 최소화하고 규제 요구 사항을 준수하면서 지연 시간을 최적화하는데 도움이 된느 리전을 고려하는 것이 중요하다.  

#### 가용 영역

-   특정 리전 내에 존재하는 데이터 센터 모음  
-   각 가용 영역은 물리적으로 고립되어 있지만 빠르고 지연 시간이 짧은 네트워크로 서로 연결되어 있다.  
-   가용 영역을 격리함으로써 다른 영역의 장애로부터 보호되고 고가용성을 보장한다.  

#### 엣지 로케이션

-   **Amazon CloudFront** 라고 하는 **CDN(콘텐츠 전송 네트워크)** 을 호스트한다. Cloud Front는 고객에게 콘텐츠를 전송하는데 사용한다.  
-   콘텐츠에 대한 요청이 가장 가까운 엣지 로케이션으로 작동 라우팅 되므로 콘텐츠가 더욱 빨리 전송되는 기술이다  

### Amazon VPC(Virtual Private Cloud)

-   Amazone VPC는 AWS 네트워킹 서비스이다.  
-   온프레미스 네트워크와 동일한 개념과 구조를 많이 사용하는 AWS 클라우드 내 프라이빗 네트워크를 생성할 수 있지만, 네트워크 설정의 복잡성 대부분이 제어, 보안 및 유용성을 희생하지 않고 추상화되었다.  
-   고객은 IP주소 공간, 서브넷 및 라우팅 테이블 같은 일반 네트워킹 구성 항목을 정의할 수 있다.  
-   VPC는 AWS 기초 서비스이며 다양한 AWS 서비스와 통합된다. (예를 들어, AC2 인스턴스는 VPC에 배포된다. Amazon RDS 데이터베이스 인스턴스는 VPC에 배포되며, 여기서 데이터베이스는 온프레미스 네트워크와 같이 네트워크 구조로 보호된다.)  
-   VPC를 이해 및 구현하면 다른 AWS 서비스를 완벽하게 사용할 수 있다.  
-   구축 : 리전 및 가용 영역의 고가용성 기반으로 구축(VPC는 한 리전 내에 상주하며 계정당 여러 VPC를 만들 수 있다.)
-   서브넷 : VPC를 나누는데 사용하며 다중 AZ에 걸쳐 구성되도록 허용한다.  
-   라우팅 테이블 : 서브넷에서 나가는 트래픽을 제어한다.  
-   인터넷 게이트웨이(IGW) : VPC에서 인터넷에 엑세스 할 수 있도록 허용.  
-   NAT 게이트웨이 : 프라이빗 서브넷 리소스가 인터넷에 엑세스하도록 허용.  
-   네트워크 엑세스 제어 목록(NACL) : 서브넷에 대한 엑세스 제어, 상태 비저장.  
-   [aws.amazon.com/VPC](aws.amazon.com/VPC)  

### 보안 그룹

-   최우선 순위이다.  
-   기본 제공되는 방화벽의 역할을 수행한다.  
-   인스턴스에 대한 엑세스 가능성을 제어
-   Source의 모든 IP 주소를 나타낼때 0.0.0.0/0으로 표시  

-->

<div align="center">

<sub><sup>Written by <a href="https://github.com/LunightLab">@Lunight</a></sup></sub><small></small>

</div>
