---

copyright:
  years:  2018, 2019
lastupdated: "2019-03-06"

keywords: Sysdig, IBM Cloud, monitoring, teams

subcollection: Sysdig

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:pre: .pre}
{:table: .aria-labeledby="caption"}
{:codeblock: .codeblock}
{:tip: .tip}
{:download: .download}
{:important: .important}
{:note: .note}

# 팀 관련 작업
{: #teams}

{{site.data.keyword.mon_full_notm}} 인스턴스의 매니저 또는 관리자는 해당 인스턴스에서 팀의 범위를 변경하고 구성원을 작성, 삭제, 추가할 수 있습니다. 
{:shortdesc} 

{{site.data.keyword.mon_full_notm}} 인스턴스의 매니저 또는 관리자는 팀을 작성하고 기존 팀을 관리하기 전에 *모니터 오퍼레이션* 팀으로 전환해야 합니다.
{: tip}

## 팀 작성
{: #teams_create}

팀을 작성하려면 다음 단계를 완료하십시오.

1. 웹 UI를 실행하십시오. 웹 UI 실행 방법에 대한 자세한 정보는 [웹 UI로 이동](/docs/services/Monitoring-with-Sysdig?topic=Sysdig-launch#launch)을 참조하십시오. 
    
2. 탐색줄의 *선택기* 단추에서 **모니터 오퍼레이션**을 선택하십시오. 그리고 **설정**을 선택하십시오.

3. **팀**을 선택하십시오. 기존 팀의 목록이 표시됩니다.

4. **팀 추가**를 클릭하십시오. 팀 구성 페이지가 표시됩니다.

5. 팀 세부사항을 구성하십시오. 

    * 색상을 선택하십시오.

    * 팀 이름을 입력하십시오.

    * [선택사항] 이 팀에 대한 설명을 입력하십시오.

    * [선택사항] 이 팀이 새 사용자의 기본 팀이 되도록 하려면 **기본 팀** 매개변수를 설정하십시오.

    * 사용자가 로그인할 때마다 열리는 웹 UI의 보기를 지정하려면 **기본 시작점**을 설정하십시오. 유효한 시작점은 *탐색* 보기, *대시보드* 보기, *이벤트* 보기, *경보* 보기 및 *설정* 보기입니다. 기본적으로 *탐색* 보기가 설정됩니다.

6. 팀 범위를 구성하십시오. 

    * [선택사항] 팀 구성원이 액세스 권한을 갖는 데이터의 레벨을 지정하려면 **범위 기준**을 설정하십시오. 유효한 값은 *호스트* 및 *컨테이너* 입니다. 매개변수가 *호스트*로 설정된 경우, 구성원은 모든 호스트 레벨과 컨테이너 레벨 정보를 볼 수 있습니다. 매개변수가 *컨테이너*로 설정된 경우, 구성원은 컨테이너 레벨 정보만 볼 수 있습니다.

    * 사용자가 볼 수 있는 데이터를 제한하려면 **범위**를 설정하십시오. 메트릭에 대한 표현식을 지정하여 하나 이상의 조건을 설정할 수 있습니다. 기본적으로 범위는 *모든 위치*로 설정됩니다.
	
    * [선택사항] **Sysdig 캡처**를 사용 또는 사용 안함으로 설정하십시오. 이 팀이 Sysdig 캡처를 작성하도록 허용하려면 이 상자를 선택하십시오. 캡처 파일은 이 팀의 구성원에게만 보입니다. **참고:** 캡처에는 팀의 범위와는 무관하게 호스트의 모든 컨테이너의 세부 정보가 포함되어 있습니다.

    * [선택사항] **인프라 이벤트**를 사용 또는 사용 안함으로 설정하십시오. 구성원이 모든 사용자 및 Sysdig 에이전트에서 모든 사용자 정의 인프라 이벤트를 볼 수 있도록 허용하려면 이 상자를 선택하십시오. 선택하지 않은 경우, 사용자는 이 팀에게 별도로 전송된 인프라 이벤트를 볼 수 있습니다. 

6. 팀에 구성원을 추가하십시오. **사용자 지정**을 클릭하십시오. 사용자를 검색하고 이를 추가하십시오.



## 팀 범위 변경
{: #teams_scope}

팀 구성원이 볼 수 있는 데이터의 범위를 변경하려면 다음 단계를 완료하십시오. 

1. 웹 UI를 실행하십시오. 웹 UI 실행 방법에 대한 자세한 정보는 [웹 UI로 이동](/docs/services/Monitoring-with-Sysdig?topic=Sysdig-launch#launch)을 참조하십시오. 
    
2. 탐색줄의 *선택기* 단추에서 **모니터 오퍼레이션**을 선택하십시오. 그리고 **설정**을 선택하십시오.

3. **팀**을 선택하십시오. 기존 팀의 목록이 표시됩니다.

4. 팀을 식별하고 이를 선택하십시오. 팀 세부사항이 표시됩니다.

5. *가시성* 섹션에서 구성 세부사항을 변경하십시오.

6. **저장**을 클릭하십시오. 


## 팀에 사용자 추가
{: #teams_users}

팀에 구성원을 추가하려면 다음 단계를 완료하십시오. 

1. 웹 UI를 실행하십시오. 웹 UI 실행 방법에 대한 자세한 정보는 [웹 UI로 이동](/docs/services/Monitoring-with-Sysdig?topic=Sysdig-launch#launch)을 참조하십시오. 
    
2. 탐색줄의 *선택기* 단추에서 **모니터 오퍼레이션**을 선택하십시오. 그리고 **설정**을 선택하십시오.

3. **팀**을 선택하십시오. 기존 팀의 목록이 표시됩니다.

4. 팀을 식별하고 이를 선택하십시오. 팀 세부사항이 표시됩니다.

5. *팀 사용자* 섹션에서 **사용자 지정**을 클릭하십시오.

6. **저장**을 클릭하십시오. 


## 팀 삭제
{: #teams_delete}

기본 팀인 **모니터 오퍼레이션**은 삭제할 수 없습니다. 

팀을 삭제하려면 다음 단계를 완료하십시오.

1. 웹 UI를 실행하십시오. 웹 UI 실행 방법에 대한 자세한 정보는 [웹 UI로 이동](/docs/services/Monitoring-with-Sysdig?topic=Sysdig-launch#launch)을 참조하십시오. 
    
2. 탐색줄의 *선택기* 단추에서 **모니터 오퍼레이션**을 선택하십시오. 그리고 **설정**을 선택하십시오.

3. **팀**을 선택하십시오. 기존 팀의 목록이 표시됩니다.

4. 삭제할 팀을 식별하고 이를 선택하십시오. 팀 세부사항이 표시됩니다.

5. **팀 삭제**를 클릭하십시오.

**참고:** 팀을 삭제하면 이 팀에만 속하는 사용자가 기본 팀으로 이동됩니다.


