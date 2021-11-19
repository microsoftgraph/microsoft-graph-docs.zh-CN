---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 68e6ba87faf8c1498cf626907e93cfd74165e83b
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61095692"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
user := msgraphsdk.NewTeamworkUserIdentity()
requestBody.SetUser(user)
user.SetAdditionalData(map[string]interface{}{
    "id": "d864e79f-a516-4d0f-9fee-0eeb4d61fdc2",
}
tenantId := "2a690434-97d9-4eed-83a6-f5f13600199a"
requestBody.SetTenantId(&tenantId)
lastMessageReadDateTime, err := time.Parse(time.RFC3339, "2021-05-27T22:13:01.577Z")
requestBody.SetLastMessageReadDateTime(&lastMessageReadDateTime)
options := &msgraphsdk.MarkChatUnreadForUserRequestBuilderPostOptions{
    Body: requestBody,
}
chatId := "chat-id"
graphClient.ChatsById(&chatId).MarkChatUnreadForUser().Post(options)


```