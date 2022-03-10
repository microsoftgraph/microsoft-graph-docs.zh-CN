---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 22cae59585dfcb2d9ffbeefe87b6becc6d7b5831
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411618"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewSubscription()
expirationDateTime, err := time.Parse(time.RFC3339, "2016-11-22T18:23:45.9356913Z")
requestBody.SetExpirationDateTime(&expirationDateTime)
options := &msgraphsdk.SubscriptionRequestBuilderPatchOptions{
    Body: requestBody,
}
subscriptionId := "subscription-id"
result, err := graphClient.SubscriptionsById(&subscriptionId).Patch(options)


```