---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f2c616657c056eb0e5f390aa1ff78e4fa1853265
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61103337"
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
graphClient.SubscriptionsById(&subscriptionId).Patch(options)


```