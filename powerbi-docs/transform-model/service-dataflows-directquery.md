---
title: Power BI(미리 보기)에서 데이터 흐름과 함께 DirectQuery 사용
description: Power BI에서 데이터 흐름과 함께 DirectQuery를 사용하는 방법 알아보기
author: davidiseminger
ms.reviewer: ''
ms.service: powerbi
ms.subservice: powerbi-service
ms.topic: conceptual
ms.date: 05/19/2020
ms.author: davidi
LocalizationGroup: Data from files
ms.openlocfilehash: 9de8c9611b24eaa627b3ddf044f13d36d7b9a3d4
ms.sourcegitcommit: 250242fd6346b60b0eda7a314944363c0bacaca8
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/20/2020
ms.locfileid: "83694576"
---
# <a name="use-directquery-with-dataflows-in-power-bi-preview"></a>Power BI(미리 보기)에서 데이터 흐름과 함께 DirectQuery 사용

DirectQuery를 사용하여 데이터 흐름에 직접 연결할 수 있으므로 관련 데이터를 가져오지 않고도 데이터 흐름에 직접 연결할 수 있습니다. 

데이터 흐름과 함께 DirectQuery를 사용하면 Power BI 및 데이터 흐름 프로세스를 다음과 같이 향상할 수 있습니다.

* **별도의 새로 고침 일정 필요 없음** - DirectQuery는 데이터 흐름에 직접 연결하므로 데이터 세트를 만들 필요가 없어집니다. 따라서 데이터 흐름과 함께 DirectQuery를 사용하면 데이터를 동기화하기 위한 데이터 흐름 및 데이터 세트의 새로 고침 일정을 별도로 만들 필요가 없습니다.

* **데이터 필터링** - DirectQuery는 데이터 흐름 내에 있는 데이터의 필터링된 보기를 작업하는 데 유용합니다. 데이터를 필터링하여 데이터 흐름 내 데이터의 작은 하위 집합으로 작업하려면 DirectQuery(및 컴퓨팅 엔진)를 사용하여 데이터 흐름 데이터를 필터링하고 필요한 필터링된 하위 집합으로 작업할 수 있습니다.


## <a name="using-directquery-for-dataflows"></a>데이터 흐름에 DirectQuery 사용

데이터 흐름과 함께 DirectQuery 사용은 2020년 5월 버전의 Power BI Desktop부터 제공되는 미리 보기 기능입니다. 

데이터 흐름과 함께 DirectQuery를 사용하기 위한 필수 조건도 있습니다.

* 데이터 흐름이 Power BI Premium 지원 작업 영역 내에 있어야 합니다.
* **컴퓨팅 엔진**이 켜져 있어야 합니다. 컴퓨팅 엔진에 대한 자세한 내용은 [향상된 컴퓨팅 엔진](service-dataflows-enhanced-compute-engine.md)을 참조하세요.

## <a name="enable-directquery-for-dataflows"></a>데이터 흐름에 DirectQuery 사용

데이터 흐름을 DirectQuery 액세스에 사용할 수 있도록 하려면 향상된 컴퓨팅 엔진이 최적화된 상태여야 합니다. 데이터 흐름에 DirectQuery를 사용하도록 설정하려면 새로운 **향상된 컴퓨팅 엔진 설정** 옵션을 **최적화됨**으로 설정합니다. 다음 이미지는 올바로 선택한 설정을 보여 줍니다.

![데이터 흐름에 향상된 컴퓨팅 엔진 사용](media/service-dataflows-directquery/dataflows-directquery-01.png)

해당 설정을 적용한 후 데이터 흐름을 새로 고쳐 최적화를 적용합니다. 


## <a name="considerations-and-limitations"></a>고려 사항 및 제한 사항

DirectQuery 및 데이터 흐름에는 다음 목록에 설명된 몇 가지 알려진 제한 사항이 있습니다.

* **향상된 메타데이터 미리 보기** 기능을 사용하도록 설정한 경우 데이터 흐름에 DirectQuery를 사용할 수 없습니다. 이 제외는 Power BI Desktop의 다음 월별 릴리스에서 제거될 예정입니다.
* 이 기능의 미리 보기 기간 중 데이터 흐름과 함께 DirectQuery를 사용하는 경우 일부 고객에게 시간 초과나 성능 문제가 발생할 수 있습니다. 이러한 문제는 미리 보기 기간 동안 적극적으로 해결됩니다.


## <a name="next-steps"></a>다음 단계

다음 문서는 데이터 흐름을 사용하는 경우에 대한 자세한 정보 및 시나리오를 참조하는 데 유용합니다.

* [데이터 흐름을 사용하여 셀프 서비스 데이터 준비](service-dataflows-overview.md)
* [Power BI Premium의 계산된 엔터티 사용](service-dataflows-computed-entities-premium.md)
* [온-프레미스 데이터 원본으로 만든 데이터 흐름 사용](service-dataflows-on-premises-gateways.md)
* [Power BI 데이터 흐름에 사용할 수 있는 개발자 리소스](service-dataflows-developer-resources.md)
* [데이터 흐름 및 Azure Data Lake 통합(미리 보기)](service-dataflows-azure-data-lake-integration.md)

공통 데이터 모델에 대한 자세한 내용은 해당 개요 문서를 참조할 수 있습니다.
* [공통 데이터 모델 - 개요 ](https://docs.microsoft.com/powerapps/common-data-model/overview)
* [GitHub에서 공통 데이터 모델 스키마 및 엔터티에 대해 자세히 알아보기](https://github.com/Microsoft/CDM)

관련된 Power BI Desktop 문서는 다음과 같습니다.

* [Power BI Desktop에서 Power BI 서비스의 데이터 세트에 연결](../connect-data/desktop-report-lifecycle-datasets.md)
* [Power BI Desktop을 사용한 쿼리 개요](desktop-query-overview.md)

관련된 Power BI 서비스 문서는 다음과 같습니다.
* [예약된 새로 고침 구성](../connect-data/refresh-scheduled-refresh.md)
