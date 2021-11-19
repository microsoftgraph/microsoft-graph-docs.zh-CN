---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0f17a1b85ffc8320ab61ab9c9d9d923a3c4bbb30
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61086076"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewChatMessage()
body := msgraphsdk.NewItemBody()
requestBody.SetBody(body)
content := "Hello world"
body.SetContent(&content)
options := &msgraphsdk.MessagesRequestBuilderPostOptions{
    Body: requestBody,
}
chatId := "chat-id"
result, err := graphClient.ChatsById(&chatId).Messages().Post(options)


```