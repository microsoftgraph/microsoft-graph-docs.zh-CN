---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c1fd78eae3db7dff2f939ca27960b101f3bccd7
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61082471"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.ChatRequestBuilderGetQueryParameters{
    Expand: "members",
}
options := &msgraphsdk.ChatRequestBuilderGetOptions{
    Q: requestParameters,
}
chatId := "chat-id"
result, err := graphClient.ChatsById(&chatId).Get(options)


```