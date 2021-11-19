---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 165fc47990d4cc6def773f6f449517f45503588e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61087742"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.TabsRequestBuilderGetQueryParameters{
    Expand: "teamsApp",
    Filter: "teamsApp/id%20eq%20'com.microsoft.teamspace.tab.web'",
}
options := &msgraphsdk.TabsRequestBuilderGetOptions{
    Q: requestParameters,
}
chatId := "chat-id"
result, err := graphClient.ChatsById(&chatId).Tabs().Get(options)


```