---
title: 보고서에서 시각적 개체 개인 설정
description: 보고서를 편집하지 않고 고유한 보고서 보기를 만듭니다.
author: mihart
ms.reviewer: ''
ms.service: powerbi
ms.subservice: powerbi-consumer
ms.topic: conceptual
ms.date: 05/09/2020
ms.author: mihart
LocalizationGroup: Reports
ms.openlocfilehash: 83f040fd021a3d3e1cd6ce344c84051c7ff58bb0
ms.sourcegitcommit: faa8cfb66e79ea16ba46605f752cc9ca57924d0e
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/13/2020
ms.locfileid: "83383160"
---
# <a name="personalize-visuals-in-a-report"></a>보고서에서 시각적 개체 개인 설정

[!INCLUDE[consumer-appliesto-ynnn](../includes/consumer-appliesto-ynnn.md)]

모든 사용자의 요구 사항을 충족하는 하나의 시각적 개체를 만드는 것은 어렵습니다. 그러나 동료가 보고서를 공유하는 경우 동료에게 변경을 요청하지 않고 직접 시각적 개체를 변경하기를 원할 수 있습니다. 

축에 있는 항목을 교환하거나, 시각적 개체 유형을 변경하거나, 도구 설명에 항목을 추가해야 할 수도 있습니다. **이 시각적 개체를 개인 설정** 기능을 사용하면 직접 시각적 개체를 변경하고 원할 경우 책갈피로 저장했다가 나중에 다시 볼 수 있습니다. 보고서에 대한 권한을 편집할 필요조차 없습니다.

:::image type="content" source="media/end-user-personalize-visuals/power-bi-personalize.png" alt-text="시각적 개체 개인 설정":::
 
## <a name="what-you-can-change"></a>변경할 수 있는 내용

이 기능을 사용하면 Power BI 보고서에서 시각적 개체 임시 탐색을 통해 추가 정보를 얻을 수 있습니다. 다음은 몇 가지 수정할 수 있는 항목입니다. 사용 가능한 옵션은 시각적 개체 유형에 따라 달라집니다. 

- 시각화 유형 변경
- 측정값 또는 차원 교환
- 범례 추가 또는 제거
- 두 개 이상의 측정값 비교
- 집계 변경 등

이 기능을 통해 새로운 탐색 기능을 사용할 수 있습니다. 또한 변경 내용을 캡처 및 공유하는 방법도 포함됩니다.

- 변경 내용 캡처
- 변경 내용 공유
- 보고서에 대한 모든 변경 내용 재설정
- 시각적 개체에 대한 모든 변경 내용 재설정
- 최근 변경 내용 지우기


## <a name="personalize-visuals-in-the-power-bi-service"></a>Power BI 서비스에서 시각적 개체 개인 설정

시각적 개체를 개인 설정하여 보고서 읽기용 보기를 종료하지 않고도 다양한 방법으로 데이터를 탐색할 수 있습니다. 다음 예제에서는 자신의 필요에 맞게 시각화를 수정할 수 있는 다양한 방법을 보여줍니다. 

1. Power BI 서비스의 읽기용 보기에서 보고서를 엽니다.

2. 시각적 개체의 메뉴 모음에서 **이 시각적 개체 개인 설정** ![이 시각적 개체 개인 설정 아이콘](media/end-user-personalize-visuals/power-bi-personalize-visual-icon.png) 아이콘을 선택합니다. 

3. **개인 설정** 필드를 모두 제거하려면 **추가 옵션(...)** 을 선택하고 **필드 제거**를 선택합니다.

### <a name="change-the-visualization-type"></a>시각화 유형 변경

데이터를 누적 세로 막대형 차트로 표시하는 것이 더 적절하다고 생각되나요? **시각화 유형**을 변경하세요.

:::image type="content" source="media/end-user-personalize-visuals/power-bi-personalize-change-visual-type.png" alt-text="시각화 유형 변경":::
 
### <a name="swap-out-a-measure-or-dimension"></a>측정값 또는 차원 교환
바꾸려는 필드를 선택한 다음 다른 필드를 선택하여 X축에 사용되는 필드를 바꿉니다.

:::image type="content" source="media/end-user-personalize-visuals/power-bi-personalize-change-axis.png" alt-text="축 변경":::
 
### <a name="add-or-remove-a-legend"></a>범례 추가 또는 제거
범례를 추가하여 범주를 기반으로 시각적 개체의 색을 구분할 수 있습니다. 이 예제에서는 회사 이름을 기준으로 색 구분을 적용합니다. 

:::image type="content" source="media/end-user-personalize-visuals/power-bi-personalize-change-legend.png" alt-text="범례 추가 또는 제거":::

### <a name="compare-two-or-more-different-measures"></a>두 개 이상의 다른 측정값 비교
\+ 아이콘으로 시각적 개체에 대한 여러 측정값을 추가하여 여러 측정값에 대한 및 대비 값을 비교합니다. 측정값을 제거하려면 **추가 옵션(...)** 을 선택하고 **필드 제거**를 선택합니다.

:::image type="content" source="media/end-user-personalize-visuals/power-bi-personalize-compare-measures.png" alt-text="측정값 비교":::

### <a name="change-aggregations"></a>집계 변경
**개인 설정** 창에서 집계를 변경하여 측정값이 계산되는 방식을 변경합니다. **추가 옵션(...)** 을 선택하고 사용할 집계를 선택합니다.

:::image type="content" source="media/end-user-personalize-visuals/power-bi-personalize-change-aggregation.png" alt-text="집계 변경":::

### <a name="capture-changes"></a>변경 내용 캡처 
개인 책갈피를 사용하여 개인 설정된 보기로 돌아갈 수 있도록 변경 내용을 캡처합니다. **책갈피** > **개인 책갈피**를 선택하고 책갈피에 이름을 지정합니다. 

:::image type="content" source="media/end-user-personalize-visuals/power-bi-personalize-bookmark.png" alt-text="책갈피 만들기":::
 
책갈피를 기본 보기로 만들 수도 있습니다.

### <a name="share-changes"></a>변경 내용 공유 
읽기 및 다시 공유 권한이 있는 경우 보고서를 공유하면 변경 내용을 포함하도록 선택할 수 있습니다.

:::image type="content" source="media/end-user-personalize-visuals/power-bi-personalize-share-changes.png" alt-text="변경 내용 공유":::
 
### <a name="reset-all-your-changes-to-a-report"></a>보고서에 대한 모든 변경 내용 재설정

보고서 캔버스의 오른쪽 위 모서리에서 **기본값으로 다시 설정**을 선택합니다. 그러면 보고서의 모든 변경 내용이 제거되고 작성자가 해당 보고서를 마지막으로 저장한 보기로 다시 설정됩니다.

:::image type="content" source="media/end-user-personalize-visuals/power-bi-personalize-reset-all.png" alt-text="모든 변경 내용 재설정":::
 
### <a name="reset-all-your-changes-to-a-visual"></a>시각적 개체에 대한 모든 변경 내용 재설정

시각적 개체의 메뉴 모음에서 **이 시각적 개체 재설정**을 선택하여 특정 시각적 개체에 대한 변경 내용을 모두 제거하고 작성자가 해당 시각적 개체를 마지막으로 저장한 보기로 재설정합니다.

:::image type="content" source="media/end-user-personalize-visuals/power-bi-personalize-reset-visual.png" alt-text="모든 시각적 변경 내용 재설정":::
 
### <a name="clear-recent-changes"></a>최근 변경 내용 지우기

**개인 설정** 창을 연 이후 변경한 최근 내용을 모두 지우려면 지우개 아이콘을 선택합니다.  

:::image type="content" source="media/end-user-personalize-visuals/power-bi-personalize-revert-changes.png" alt-text="최근 변경 내용 되돌리기":::

## <a name="limitations-and-known-issues"></a>제한 사항 및 알려진 문제

현재 이 기능에는 몇 가지 주의 사항이 있습니다.

- **이 시각적 개체 개인 설정**은 전체 보고서 또는 특정 시각적 개체에 대해 해제할 수 있습니다. 시각적 개체를 개인 설정할 수 있는 옵션이 없는 경우 테넌트 관리자 또는 보고서 소유자에게 문의하세요. 보고서 소유자의 연락처 정보를 표시하려면 Power BI 메뉴 모음에서 보고서 이름을 선택합니다.
- 사용자 탐색은 자동으로 유지되지 않습니다. 변경 내용을 캡처하려면 개인 책갈피로 보기를 저장해야 합니다.
- Power BI 모바일 앱에 있는 동안에는 시각적 개체를 변경할 수 없습니다. 그러나 Power BI 서비스 중에 개인 책갈피에 저장한 시각적 개체 변경 내용은 모바일 앱에서 적용됩니다.

또한 해결 중인 알려진 문제가 몇 가지 있습니다.

- 계층 구조 추가는 지원되지 않습니다. 개별 자식 항목을 각각 추가해야 합니다.
- 개인 책갈피를 사용하면 선택한 시퀀스에 따라 약간 다른 결과를 얻을 수 있습니다. 보고서의 전체 상태가 아닌 수정된 내용만 캡처하기 때문에 불일치가 발생할 수 있습니다. 해결 방법으로 **기본으로 재설정**을 선택하고 볼 책갈피를 선택합니다. 

## <a name="next-steps"></a>다음 단계
[보고서 시각적 개체를 정적 이미지로 복사](../visuals/power-bi-visualization-copy-paste.md)    
궁금한 점이 더 있나요? [Power BI 커뮤니티를 이용하세요.](https://community.powerbi.com/)

