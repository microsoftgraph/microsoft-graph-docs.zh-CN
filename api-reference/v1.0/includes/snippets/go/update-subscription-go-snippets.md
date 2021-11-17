---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e123b0685fa7289c62d540f704fad8afc746994a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61030568"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewSubscription()
expirationDateTime, err := time.Parse(time.RFC3339, "2016-11-22T18:23:45.9356913Z")
requestBody.SetExpirationDateTime(&expirationDateTime)
options := &msgraphsdk.SubscriptionRequestBuilderPatchOptions{
    Body: requestBody,
}
subscriptionId := "subscription-id"
graphClient.SubscriptionsById(&subscriptionId).Patch(options)


```