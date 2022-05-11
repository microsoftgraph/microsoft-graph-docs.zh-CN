---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f763e7a9f20ff182bb713c2232aa82759685c693
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65329052"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.InstalledAppsRequestBuilderGetQueryParameters{
    Expand: "teamsApp,teamsAppDefinition",
    Filter: "teamsApp/externalId%20eq%20'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'",
}
options := &msgraphsdk.InstalledAppsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
chatId := "chat-id"
result, err := graphClient.ChatsById(&chatId).InstalledApps().GetWithRequestConfigurationAndResponseHandler(options, nil)


```