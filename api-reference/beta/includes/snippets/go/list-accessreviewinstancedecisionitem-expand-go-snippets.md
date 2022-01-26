---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 29c3eb3906ba8441ce532f84a1e4cb3f7d8d3a64
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2022
ms.locfileid: "62224913"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.AccessReviewInstanceDecisionItemRequestBuilderGetQueryParameters{
    Expand: "instance($expand=definition)",
}
options := &msgraphsdk.AccessReviewInstanceDecisionItemRequestBuilderGetOptions{
    Q: requestParameters,
}
accessReviewInstanceDecisionItemId := "accessReviewInstanceDecisionItem-id"
result, err := graphClient.IdentityGovernance().AccessReviews().DecisionsById(&accessReviewInstanceDecisionItemId).Get(options)


```