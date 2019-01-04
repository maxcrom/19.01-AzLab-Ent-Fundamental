![](media/image1.png){width="2.1770833333333335in"
height="0.7256944444444444in"}

> **Microsoft Azure 인프라 & 솔루션 과정**

Lab 1

가상 머신 만들기

Update : 2018.V5

Overview

이번 실습에서는 금일 실습에서 사용될 Microsoft Azure 의 기본 환경을
구성한 후, 포털에서 가상 머신(Virtual Machine, VM)를 만들어 봅니다.

이번 실습에서는 실습 환경 구성을 위해, 아래 사항들을 진행합니다.

> 가상 머신 (가상 머신)을 생성합니다.
>
> Option : Azure PowerShell을 설치 합니다.

Lab 1: 실습 환경 준비

**이번 실습의 작업들**

> 실습환경준비- Azure Pass 활성화

Azure 포털을 이용한 가상 머신 만들기

> Windows PowerShell 의 Microsoft Azure 모듈 설치

**[\<Microsoft Azure Pass 등록 및 구독 활성화\>]{.underline}**

1.  개월간 무료로 사용할 수 있는 Microsoft Azure Pass 를 사용자
    계정(Microsoft Account)에 등록합니다.

**모든 웹 브라우저를 종료하고 새로 열거나, InPrivate 브라우징으로 기존
세션과 연결되지 않은 웹 브라우저 환경에서 합니다. **

**[Outlook.com에서 계정 생성 진행을 하면서 "Too Many Request" 메시지가
나타나서 안 될 경우, 스마트폰에서 계정 생성을 진행합니다.]{.underline}**

1\. [[http://Outlook.com]{.underline}](http://Outlook.com) 사이트에 접속
후 **\[가입\]**을 클릭하고 계정을 생성합니다.

![](media/image2.png){width="4.5154779090113735in" height="2.275in"}

![](media/image3.png){width="4.1in" height="2.311111111111111in"}

2\. 브라우저를 통해
[[https://www.microsoftazurepass.com/](http://aka.ms/kpass)]{.underline}
사이트에 접속 하고 **\[Start\]**를 클릭합니다.

![](media/image4.png){width="3.9583333333333335in"
height="3.013624234470691in"}

3\. 앞에서 만든 Outlook 계정으로 로그인을 합니다.

![](media/image5.png){width="3.966666666666667in"
height="2.287212379702537in"}

4\. 계정 정보가 맞는지 확인하고, **\[Confirm Microsoft Account\]**를
클릭합니다.

![](media/image6.png){width="5.255905511811024in"
height="2.578740157480315in"}

5\. 전달 받은 Code를 입력하고, **\[Claim Promo Code\]**를 클릭합니다.

![](media/image7.png){width="6.55in" height="2.875in"}

> 6\. **\[Activate\]**를 클릭합니다. 이후 필요한 정보만 입력하고
> **\[다음\]**을 클릭합니다.
>
> ![](media/image8.png){width="4.358267716535433in"
> height="2.574803149606299in"}
>
> ![](media/image9.png){width="4.925196850393701in"
> height="3.322834645669291in"}
>
> 7\. 전화번호를 입력합니다.
>
> ![](media/image10.png){width="5.791666666666667in"
> height="2.7937171916010497in"}

8\. 체크 박스를 클릭하고 **\[등록\]**을 누르면 약 5분 정도 기다립니다.

![](media/image11.png){width="6.766666666666667in"
height="2.79667760279965in"}

> **9.** Microsoft Azure 구독 생성이 완료되었습니다.

![](media/image12.png){width="6.625574146981627in"
height="5.10877624671916in"}

Microsoft Azure 포털의 주소는
[[http://portal.azure.com]{.underline}](http://portal.azure.com/)
입니다.

**[\<Azure Portal을 이용한 가상 머신 만들기\>]{.underline}**

1\. Azure 포털에서 **\[+ 리소스 만들기\]**를 클릭하고, **\[Windows Server
2016 VM\]**을 클릭합니다.

![](media/image13.png){width="5.878087270341207in"
height="3.0411450131233595in"}

2\. 기본 사항에 필요한 항목을 입력합니다.

**구독:** 현재 사용 가능한 구독

**리소스 그룹**: 새로 만들기 -\> **userXX-lab1-rg**

**가상 머신 이름**: **userXX-lab1-vm**

**지역: 예) 미국 서부 2**

**가용성 옵션: "인프라 중복이 필요하지 않습니다." 선택**

**이미지 : Windows Server 2016 Datacenter**

**크기 : "크기 변경" 클릭 후 "D2\_v3 (표준)"을 클릭**

**사용자 이름** (컴퓨터 로그인 계정) : 임의의 계정 (예: **iaasadmin**)

**암호** : **임의의 암호 12자리**

**암호 확인** : 동일한 암호 입력

**공용 인바운드 포트**: "**선택한 포트 허용**" 클릭 후 "**RDP
(3389)**"를 클릭

이미 Windows 라이선스가 있나요? : **아니오**

위의 항목까지 입력하고 **\[검토 + 만들기\]**를 클릭합니다.

![](media/image14.png){width="6.268055555555556in"
height="6.268055555555556in"} (예제화면)

3\. 앞에서 설정한 값을 확인하고, **\[만들기\]**를 클릭합니다.

![](media/image15.png){width="5.171103455818023in"
height="5.73043416447944in"}

4\. 약 10분정도 기다리면 가상 머신 (가상 머신) 생성이 완료됩니다.

5\. Azure 포털에서 **\[가상 머신\]**을 클릭합니다.
![](media/image16.png){width="1.458150699912511in"
height="0.4270297462817148in"}

6\. 가상머신 **\[userXX-lab1-vm\]**을 클릭하고 **\[연결\]**을 클릭한
다음, **\[RDP 파일 다운로드\]**를 클릭합니다.\
그리고 RDP파일을 **\[열기\]**를 클릭합니다.

![](media/image17.png){width="9.511805555555556in"
height="3.5541666666666667in"}

7\. 앞에서 입력했던 **사용자 이름 / 암호**를 입력하고 **\[확인\]**을
클릭합니다.

![](media/image18.png){width="3.6173917322834646in"
height="2.792373140857393in"}

8\. 로그인이 완료 되면 서버에 접속이 된 것을 확인 할 수 있습니다.

![](media/image19.png){width="9.511805555555556in"
height="5.040972222222222in"}

**[\< Windows PowerShell 의 Microsoft Azure 모듈 설치 \>]{.underline}**

Windows PowerShell 에서 사용하게 될 Microsoft Azure 모듈을 설치합니다.

1\. 실습 컴퓨터의 웹 브라우저에서 다음 주소에 접속합니다.
[**[https://azure.microsoft.com/ko-kr/downloads/]{.underline}**](https://azure.microsoft.com/ko-kr/downloads/)

> *이 링크는 Microsoft Azure 관련 도구들을 다운로드 받을 수 있는
> 사이트입니다.*

2\. 웹 페이지 중단에 위치한 **명령줄 도구** 분류의 **PowerShell** 아래
**Windows 설치**를 클릭합니다.

![](media/image20.png){width="4.958333333333333in"
height="3.34586832895888in"}

3\. 아래와 같이 팝업창에서 **실행**을 선택합니다.

![](media/image21.png){width="6.3in" height="0.5165288713910761in"}

4\. 열리는 웹 플랫폼 설치 관리자 5.0 창에서 **설치**를 선택합니다.

![](media/image22.png){width="4.7183770778652665in"
height="3.3020833333333335in"}

5\. 필수 구성 요소 창에서 **동의함**을 선택합니다.

> *웹 플랫폼 설치 관리자가 Microsoft Azure PowerShell 모듈을 설치하게
> 됩니다*.

![](media/image23.png){width="4.0625in" height="2.801110017497813in"}

필수 구성 요소 페이지에서 사용하는 Windows 의 설정에 따라 설치합니다.

6\. 설치가 완료되면 **마침**을 클릭합니다.

![](media/image24.png){width="4.382280183727034in" height="2.40625in"}

7\. 시작버튼에서 마우스 우 클릭을 하고, **Windows PowerShell(관리자)**를
실행합니다.

![](media/image25.png){width="2.84375in" height="3.738740157480315in"}

8\. PowerShell 의 명령 프롬프트에 다음 명령어를 입력 합니다.
**Add-AzureRMA****ccount**

(Add-AzureRMA 까지만 입력하고 Tap 키를 누르면 명령어가 나와야 합니다.\
간혹 설치 직후에 안 나오는 경우가 있는데, 이런 경우는 실습 PC를 재부팅을
해보시기 바랍니다.)

![](media/image26.png){width="4.114583333333333in"
height="0.36775590551181103in"}

9\. Microsoft Azure 포털 로그인시 사용했던 계정을 사용하여 로그인합니다.

![](media/image27.png){width="4.2in" height="2.526175634295713in"}

10\. PowerShell 창에서 아래 명령어를 입력하여 구독 정보를 확인합니다.\
**Get-AzureRmSubscription**

![](media/image28.png){width="4.45829615048119in" height="1.025in"}
\<예제화면\>

> 11\. **(선택, 만약 위에서 구독이 여러 개인 경우에만)\
> **PowerShell 에서 관리할 구독을 선택하기 위해서는 다음 PowerShell
> 명령어를 사용합니다.
>
> Select-AzureRmSubscription -SubscriptionID **"SUBSCRIPTION ID"**
>
> *Subscription ID 는 PowerShell 에서 선택하여 복사 후 붙여넣기 할 수
> 있습니다.*

\<참고\> 만일 Azure PowerShell이 동작하지 않을 경우,

파워쉘에서 **Import-module azurerm** 을 입력해서

Azure Powershell 모듈을 import 해야 합니다.
