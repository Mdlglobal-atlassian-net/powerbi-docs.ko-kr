---
title: 타일 오류 문제 해결
description: 타일이 Power BI에서 새로 고쳐질 때 발생할 수 있는 일반적인 오류
author: maggiesMSFT
ms.reviewer: kayu
ms.custom: seodec18
ms.service: powerbi
ms.subservice: powerbi-service
ms.topic: troubleshooting
ms.date: 12/06/2018
ms.author: maggies
LocalizationGroup: Troubleshooting
ms.openlocfilehash: 463275d98c72441264e5bae699d983eb34bb1058
ms.sourcegitcommit: 0e9e211082eca7fd939803e0cd9c6b114af2f90a
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/13/2020
ms.locfileid: "83320495"
---
# <a name="troubleshooting-tile-errors"></a>타일 오류 문제 해결
다음은 설명이 있는 타일에 발생할 수 있는 일반적인 오류입니다.

> [!NOTE]
> 아래 나열되어 있지 않은 오류가 발생하고 문제를 발생시킨 경우 [커뮤니티 사이트](https://community.powerbi.com/)에 추가 지원을 요청하거나 [지원 티켓](https://powerbi.microsoft.com/support/)을 만들 수 있습니다.
> 
> 

## <a name="errors"></a>오류
**Power BI에서 모델을 로드하는 동안 예기치 않은 오류가 발생했습니다. 나중에 다시 시도하세요.**
또는 **데이터 모델을 검색할 수 없습니다. 대시보드 소유자에게 문의하여 데이터 소스 및 모델이 존재하고 액세스 가능한지 확인하세요.**

데이터 원본을 연결할 수 없기 때문에 데이터에 액세스할 수 없습니다. 이 문제는 데이터 원본이 제거되거나 이름이 변경되고 이동하거나 오프라인 상태 또는 사용 권한이 변경되는 경우 발생할 수 있습니다. 원본이 아직 가리키는 위치에 있고 아직 액세스할 권한이 있는지 확인합니다. 이것이 문제가 아니면 원본이 느려질 수 있습니다. 원본의 부하가 더 작아질 때 다시 시도합니다. 온-프레미스 원본인 경우 데이터 원본 소유자는 자세한 정보를 제공할 수 있습니다.

**이 타일을 보거나 통합 문서를 열 권한이 없습니다.**

대시보드 소유자에게 문의하여 데이터 원본 및 모델이 존재하고 해당 계정으로 액세스할 수 있는지 확인하세요.

**Power BI 시각적 개체가 관리자에 의해 사용하지 않도록 설정되었습니다.**

Power BI 관리자가 조직 또는 보안 그룹에 대한 Power BI 시각적 개체를 사용하지 않도록 설정했습니다.
[Microsoft 마켓플레이스](https://appsource.microsoft.com/marketplace/apps?page=1&product=power-bi-visuals)에서 Power BI 시각적 개체를 사용하거나 파일에서 프라이빗 시각적 개체를 가져올 수 없습니다. 사전 압축된 시각적 개체 집합만 사용할 수 있습니다.


**데이터 셰이프에는 하나 이상의 그룹이나 데이터를 출력하는 계산이 포함되어야 합니다. 대시보드 소유자에게 문의하세요.**

쿼리가 비어 있기 때문에 데이터를 표시하지 않습니다. 필드 목록에서 시각적 개체로 일부 필드를 추가하고 다시 열어 봅니다.

**Power BI에서 둘 이상의 필드 간 관계를 확인할 수 없으므로 데이터를 표시할 수 없습니다.**

관련되지 않은 테이블에서 두 개 이상의 필드를 사용하려고 합니다. 시각적 개체에서 관련이 없는 필드를 제거하고 테이블 간의 관계를 만들어야 합니다. 이 변경 작업을 완료하면 시각적 개체에 다시 필드를 추가할 수 있습니다. Power BI Desktop 또는 Excel용 파워 피벗에서 수행할 수 있습니다. [자세히 알아보기](../transform-model/desktop-create-and-manage-relationships.md)

**기본 축과 보조 축의 그룹이 겹칩니다. 기본 축의 그룹은 보조 축의 그룹과 동일한 키를 가질 수 없습니다.**

이는 일반적으로 일시적인 문제입니다. 일반적으로 그룹을 행에서 열로 이동할 때 발생합니다. 이 경우에 모든 그룹의 이동을 마치면 오류가 사라져야 합니다. 메시지가 계속 나타나면 행과 열 또는 축 범례 사이의 필드를 전환하거나 시각적 개체의 필드를 제거해 봅니다.  

**이 시각적 개체는 사용 가능한 리소스를 초과했습니다. 표시되는 데이터 양을 줄이려면 필터링을 시도합니다.**

시각적 개체는 사용 가능한 리소스로 결과를 완료하기에 너무 많은 데이터를 쿼리하려 했습니다. 시각적 개체를 필터링하여 결과에서 데이터의 양을 줄입니다.

**다음 필드를 식별할 수 없습니다. {0} 데이터 세트에 존재하는 필드를 사용하여 시각적 개체를 업데이트합니다.**

필드가 삭제되었거나 이름이 바뀌었을 수 있습니다. 시각적 개체에서 끊어진 필드를 제거하고 다른 필드를 추가하며 다시 고정할 수 있습니다.

**이 시각적 개체에 대한 데이터를 검색할 수 없습니다. 나중에 다시 시도하세요.**

일반적으로 일시적인 문제가 있습니다. 나중에 다시 시도해도 이 메시지가 계속 표시되면 지원팀에 문의하세요.

**타일이 SSO(Single Sign-On)를 사용하도록 설정한 후에도 계속 필터링되지 않은 데이터를 표시합니다.**

기본 데이터 세트가 DirectQuery 모드 또는 라이브 연결을 사용하여 온-프레미스 데이터 게이트웨이를 통해 Analysis Services에 연결하도록 구성된 경우 이런 현상이 발생할 수 있습니다. 이런 경우, 다음 타일 새로 고침이 도래할 때까지는 타일이 데이터 원본에 대해 SSO를 사용하도록 설정한 후에도 계속 필터링되지 않은 데이터를 표시합니다. 다음 타일 새로 고침 시에는, Power BI가 구성된 대로 SSO를 사용하고 타일이 사용자 ID에 따라 필터링된 데이터를 표시합니다. 

필터링된 데이터를 즉시 보려는 경우, 대시보드의 오른쪽 위에 있는 **추가 옵션**(...)을 선택하고 **대시보드 타일 새로 고침**을 선택하여 타일 새로 고침을 강제로 적용할 수 있습니다.

데이터세트 소유자는 타일 새로 고침 빈도를 변경하고 15분으로 설정하여 타일 새로 고침을 가속화할 수도 있습니다. Power BI 서비스의 오른쪽 위 모퉁이에서 기어 아이콘을 선택한 다음 **설정**을 선택합니다. **설정** 페이지에서 **데이터 세트** 탭을 선택합니다. **예약된 캐시 새로 고침**을 확장하고 **새로 고침 빈도**를 변경합니다. Power BI가 다음 타일 새로 고침을 수행한 후에 원래 새로 고침 빈도로 구성을 재설정해야 합니다.

> [!NOTE]
> **예약된 캐시 새로 고침** 섹션은 DirectQuery/라이브 연결 모드의 데이터 세트에 대해서만 사용할 수 있습니다. 타일이 다음 예약된 데이터 새로 고침 동안 자동으로 새로 고쳐지기 때문에 가져오기 모드의 데이터 세트는 별도의 타일 새로 고침이 필요하지 않습니다.

## <a name="contact-support"></a>지원 문의
문제가 여전히 발생하는 경우 더 자세히 조사하기 위해 [지원팀에 문의](https://support.powerbi.com)합니다.

## <a name="next-steps"></a>다음 단계
[온-프레미스 데이터 게이트웨이 문제 해결](service-gateway-onprem-tshoot.md)  
[Power BI Personal Gateway 문제해결](service-admin-troubleshooting-power-bi-personal-gateway.md)  
궁금한 점이 더 있나요? [Power BI 커뮤니티를 이용하세요.](https://community.powerbi.com/)