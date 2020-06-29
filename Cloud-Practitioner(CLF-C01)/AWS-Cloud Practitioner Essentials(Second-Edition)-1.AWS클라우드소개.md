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

**<div align=right> Introduction to the AWS Cloud</div>**

### AWS 클라우드 소개

-	AWS를 통해 서버, 데이터베이스, 스토리지 및 상위 애플리케이션 구성요소를 몇 초 이내에 엑세스 할 수 있다.
-	임시 또는 일회용 리소스로 취급할 수 있어 고정적이고 유한한 IT인프라를 경직성과 제약으로부터 자유로울 수 있다.  

### AWS 클라우드 특성

**민첩성 (Agility)**

-	**속도(Speed)** : 막대한 투자와 비용이 필요없이 전세계 네트워크에 빠르게 서비스가 가능  
-	**실험(Experimentation)** : 클라우드 환경을 통해 실험을 자주 할 수 있으며 빈번한 실험을 통해 새로운 구성과 탐색이 가능하다.  
-	**혁신의 문화 (Culture of innovation)**  
-	**CloudFormation** 을 통해 일관적이고 템플릿화된 개발 환경 구축이 가능하다.  
	*CloudFormation - AWS에서 제공하는 템플릿이나 개발자 혹은 시스템 관리자가 작성한 템플릿을 이용해 AWS 리소스들을 쉽게 생성하고 관리하는 방법을 제공한다.*

**내결함성**

-	시스템 구성 요소에 장애가 발생하더라도 시스템이 작동 가능 상태를 유지하는 능력(애플리케이션 구성 요소의 기본적인 중복성)

**고가용성**

-	사용자 개입 없이 시스템이 항상 자동으로 액세스 가능하며 가동 중지가 최소화되도록 하는 능력

**탄력성**

-	간편하게 컴퓨팅 리소스의 규모를 확장하거나 축소할 수 있는 능력  

### AWS 관리 인터페이스

AWS 사용자는 AWS Management Consle, AWS 명령줄 인터페이스(AWS CLI), AWS SDK(AWs Software development kiet)를 사용하여 고유한 방법으로 리소스를 만들고 관리할 수 있다. 이 세가지 옵션은 공통 인터페이스 또는 APIF를 기반으로 한다.

**AWS Management Console**

-	AWS기능에 엑세스할 수 있는 그래픽 인터페이스를 제공.  
-	다양한 AWS 서비스 및 기능을 열고 사용할 수 있다.  
-	iOS 또는 Android 플랫폼에서 사용할 수 있도록 App을 제공하고 기존 리소스 및 경보를 보고 편리하게 운영 작업을 수행할 수 있다.  

**AWS CLI**

-	명령중에러 AWS서비스를 제어할 수 있다.  
-	언어에 관계없는 프로그래밍 방식으로 AWS리소스 배포를 자동화하고 반복할 수 있다.  
-	Windows, Linux, MacOS 또는 Unix 명령 실행을 포함하며 AWS의 모든 기능을 사용할 수 있다.  

**AWS SDK**

-	다양한 인기 프로그래밍 언어를 사용하여 기존 애플리케이션에서 AWS를 사용할 수 있는 위치에서 코드만 사용하여 복잡한 시스템을 배포하고 모니터링 할 수 있는 애플리케이션이다.  
-	AWS CLI 및 SDK를 사용하면 AWS 기능을 사용자 지정하고 비즈니스와 관련된 고유 도구를 유연하게 생성할 수 있다.  
-	언어별 SDK에 직접 어렵게 함수를 작성하지 않고 다양한 AWS 클라우드 서비스의 연결 및 기능을 코드에 쉽게 통합할 수 있는 API가 포함되어 있다.  

위 세가지는 교대로 사용가능하다. 예로 SDK에 호출하여 EC2 인스턴스를 생성한 다음, 이를 확인하고, 나중에 CLI를 사용하여 콘솔에서 종료가 가능하다.

<div align="center">

<sub><sup>Written by <a href="https://github.com/LunightLab">@Lunight</a></sup></sub><small></small>

</div>
