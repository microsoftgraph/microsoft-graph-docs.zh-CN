---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1477266b786dfe93800686abb179ed70c2913b48
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65314521"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.AccessReviewsRequestBuilderGetQueryParameters{
    Filter: "businessFlowTemplateId%20eq%20'6e4f3d20-c5c3-407f-9695-8460952bcc68'",
    Top: 100,
    Skip: 0,
}
options := &msgraphsdk.AccessReviewsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.AccessReviews().GetWithRequestConfigurationAndResponseHandler(options, nil)


```