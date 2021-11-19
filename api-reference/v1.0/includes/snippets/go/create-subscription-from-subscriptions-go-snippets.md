---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d8dacbd9bd7bcf2172ea14a82e6079750c4b0a9e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088407"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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