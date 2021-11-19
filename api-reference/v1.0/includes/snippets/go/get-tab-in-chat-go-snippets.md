---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9d27a1bb3bdc6275f47cebe41ed6f6041b9ab3a1
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61098078"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.TeamsTabRequestBuilderGetQueryParameters{
    Expand: "teamsApp",
}
options := &msgraphsdk.TeamsTabRequestBuilderGetOptions{
    Q: requestParameters,
}
chatId := "chat-id"
teamsTabId := "teamsTab-id"
result, err := graphClient.ChatsById(&chatId).TabsById(&teamsTabId).Get(options)


```