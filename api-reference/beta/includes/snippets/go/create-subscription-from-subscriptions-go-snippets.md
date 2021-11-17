---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce7df1b7fb0793542d072122207c8fc36ad9fad6
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61010693"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewSubscription()
changeType := "created"
requestBody.SetChangeType(&changeType)
notificationUrl := "https://webhook.azurewebsites.net/api/send/myNotifyClient"
requestBody.SetNotificationUrl(&notificationUrl)
resource := "me/mailFolders('Inbox')/messages"
requestBody.SetResource(&resource)
expirationDateTime, err := time.Parse(time.RFC3339, "2016-11-20T18:23:45.9356913Z")
requestBody.SetExpirationDateTime(&expirationDateTime)
clientState := "secretClientValue"
requestBody.SetClientState(&clientState)
latestSupportedTlsVersion := "v1_2"
requestBody.SetLatestSupportedTlsVersion(&latestSupportedTlsVersion)
options := &msgraphsdk.SubscriptionsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Subscriptions().Post(options)


```