---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae3d01632fee12e643a078a438a536d5b004c965
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089923"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.DecisionsRequestBuilderGetQueryParameters{
    Top: 100,
    Skip: 0,
}
options := &msgraphsdk.DecisionsRequestBuilderGetOptions{
    Q: requestParameters,
}
accessReviewInstanceId := "accessReviewInstance-id"
result, err := graphClient.Me().PendingAccessReviewInstancesById(&accessReviewInstanceId).Decisions().Get(options)


```