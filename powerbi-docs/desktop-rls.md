---
title: Power BI Desktop에 대해 RLS(행 수준 보안)를 사용하여 데이터 액세스 제한
description: Power BI Desktop 내에서 가져온 데이터 세트 및 DirectQuery에 대한 행 수준 보안을 구성하는 방법입니다.
author: davidiseminger
ms.author: davidi
ms.reviewer: ''
ms.service: powerbi
ms.subservice: powerbi-desktop
ms.topic: conceptual
ms.custom: ''
ms.date: 01/31/2020
LocalizationGroup: Create reports
ms.openlocfilehash: 7a9aa0ca62ae4f1008d4cf47caa909841f9ec495
ms.sourcegitcommit: 7aa0136f93f88516f97ddd8031ccac5d07863b92
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/05/2020
ms.locfileid: "77464479"
---
# <a name="restrict-data-access-with-row-level-security-rls-for-power-bi-desktop"></a>Power BI Desktop에 대해 RLS(행 수준 보안)를 사용하여 데이터 액세스 제한

Power BI Desktop에서 RLS(행 수준 보안)를 사용하여 지정된 사용자의 데이터 액세스를 제한할 수 있습니다. 행 수준에서 데이터 제한을 필터링합니다. 역할 내에서 필터를 정의할 수 있습니다.

이제 Power BI Desktop으로 Power BI로 가져온 데이터 모델에 대한 RLS를 구성할 수 있습니다. SQL Server와 같은 [DirectQuery](desktop-use-directquery.md)를 사용하는 데이터 세트에서 RLS를 구성할 수도 있습니다. 이전에는 Power BI 외부의 온-프레미스 Analysis Services 모델 내에서만 RLS를 구현할 수 있었습니다. Analysis Services 라이브 연결의 경우 온-프레미스 모델에서 행 수준 보안을 구성합니다. 라이브 연결 데이터 세트에는 보안 옵션이 표시되지 않습니다.

> [!IMPORTANT]
> Power BI 서비스 내에서 역할과 규칙을 정의한 경우 Power BI Desktop 내에서 해당 역할을 다시 만든 다음, 보고서를 서비스에 게시해야 합니다. [Power BI 서비스 내에서 RLS](service-admin-rls.md) 옵션에 대해 자세히 알아보세요.

[!INCLUDE [include-short-name](./includes/rls-desktop-define-roles.md)]

[!INCLUDE [include-short-name](./includes/rls-desktop-view-as-roles.md)]

[!INCLUDE [include-short-name](./includes/rls-limitations.md)]

[!INCLUDE [include-short-name](./includes/rls-faq.md)]

## <a name="next-steps"></a>다음 단계

[Power BI 서비스를 사용하는 행 수준 보안(RLS)](service-admin-rls.md)  

궁금한 점이 더 있나요? [Power BI 커뮤니티에 질문합니다](https://community.powerbi.com/).