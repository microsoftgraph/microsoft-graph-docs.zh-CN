---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d05018264e10b1f580cf19273e0b238bed3c78c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328912"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewSubscription()
expirationDateTime, err := time.Parse(time.RFC3339, "2016-11-22T18:23:45.9356913Z")
requestBody.SetExpirationDateTime(&expirationDateTime)
subscriptionId := "subscription-id"
graphClient.SubscriptionsById(&subscriptionId).Patch(requestBody)


```