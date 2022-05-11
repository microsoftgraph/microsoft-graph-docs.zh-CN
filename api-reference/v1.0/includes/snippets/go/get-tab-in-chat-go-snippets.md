---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9709820a0b8a5698b8e3c1f05ca4364a65251709
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328552"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.TeamsTabRequestBuilderGetQueryParameters{
    Expand: "teamsApp",
}
options := &msgraphsdk.TeamsTabRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
chatId := "chat-id"
teamsTabId := "teamsTab-id"
result, err := graphClient.ChatsById(&chatId).TabsById(&teamsTabId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```