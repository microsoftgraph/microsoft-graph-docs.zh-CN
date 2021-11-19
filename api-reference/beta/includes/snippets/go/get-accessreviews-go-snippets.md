---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 70a1e4dcc915689bcf6803794b2dbaf070f6aef2
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61100474"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.AccessReviewsRequestBuilderGetQueryParameters{
    Filter: "businessFlowTemplateId%20eq%20'6e4f3d20-c5c3-407f-9695-8460952bcc68'",
    Top: 100,
    Skip: 0,
}
options := &msgraphsdk.AccessReviewsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.AccessReviews().Get(options)


```