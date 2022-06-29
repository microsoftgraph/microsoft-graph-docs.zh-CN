---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8f894e7ae5b755dbed789d03297d915e628ee943
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65693865"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPinnedChatMessageInfo()
requestBody.SetAdditionalData(map[string]interface{}{
    "message@odata.bind": "https://graph.microsoft.com/beta/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages/1616964509832",
}
chatId := "chat-id"
result, err := graphClient.ChatsById(&chatId).PinnedMessages().Post(requestBody)


```