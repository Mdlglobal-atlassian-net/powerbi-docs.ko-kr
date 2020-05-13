---
title: Power BI 시각적 개체에 방문 페이지 추가
description: 이 문서에서는 Power BI 시각적 개체에 방문 페이지를 추가하는 방법을 설명합니다.
author: KesemSharabi
ms.author: kesharab
ms.reviewer: sranins
ms.service: powerbi
ms.subservice: powerbi-custom-visuals
ms.topic: reference
ms.date: 06/18/2019
ms.openlocfilehash: 6f1590d5635ed6e55833350027c52379e5d7cf51
ms.sourcegitcommit: 7aa0136f93f88516f97ddd8031ccac5d07863b92
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/05/2020
ms.locfileid: "79379966"
---
# <a name="add-a-landing-page-to-your-power-bi-visuals"></a>Power BI 시각적 개체에 방문 페이지 추가

API 2.3.0에서는 Power BI 시각적 개체에 방문 페이지를 추가할 수 있습니다. 기능에 `supportsLandingPage`를 추가하고 true로 설정하면 됩니다. 이 작업을 수행하면 데이터를 추가하기 전에 시각적 개체가 초기화되고 업데이트됩니다. 시각적 개체에 더 이상 워터마크가 표시되지 않으므로, 데이터가 없을 경우 시각적 개체에 표시할 고유한 방문 페이지를 디자인할 수 있습니다.

```typescript
export class BarChart implements IVisual {
    //...
    private element: HTMLElement;
    private isLandingPageOn: boolean;
    private LandingPageRemoved: boolean;
    private LandingPage: d3.Selection<any>;

    constructor(options: VisualConstructorOptions) {
            //...
            this.element = options.element;
            //...
    }

    public update(options: VisualUpdateOptions) {
    //...
        this.HandleLandingPage(options);
    }

    private HandleLandingPage(options: VisualUpdateOptions) {
        if(!options.dataViews || !options.dataViews.length) {
            if(!this.isLandingPageOn) {
                this.isLandingPageOn = true;
                const SampleLandingPage: Element = this.createSampleLandingPage(); //create a landing page
                this.element.appendChild(SampleLandingPage);
                this.LandingPage = d3.select(SampleLandingPage);
            }

        } else {
                if(this.isLandingPageOn && !this.LandingPageRemoved){
                    this.LandingPageRemoved = true;
                    this.LandingPage.remove();
                }
        }
    }
```

다음 그림은 예제 방문 페이지를 보여 줍니다.

![방문 페이지 스크린샷](media/landing-page/app-landing-page.png)
