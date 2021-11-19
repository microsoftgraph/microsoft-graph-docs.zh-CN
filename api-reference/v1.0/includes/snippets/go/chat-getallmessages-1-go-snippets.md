---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f2217a8b5bde85a1686ea01805695d60b22fd7b7
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61086112"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.ChatRequestBuilderGetQueryParameters{
    Top: 2,
}
options := &msgraphsdk.ChatRequestBuilderGetOptions{
    Q: requestParameters,
}
userId := "user-id"
chatId := "chat-id"
result, err := graphClient.UsersById(&userId).ChatsById(&chatId).Get(options)


```