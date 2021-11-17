---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5a5b4ae6f64fccc90bf251b8d66d9fc73a1b98ff
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60996595"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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