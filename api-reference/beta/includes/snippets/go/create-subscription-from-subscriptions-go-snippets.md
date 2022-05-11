---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d9251bda079cc9ab6043086929e8367c6e7b9a12
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325838"
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
result, err := graphClient.Subscriptions().Post(requestBody)


```