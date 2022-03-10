---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2bce47d008606823f8b6faaaf891ca8faef23da1
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411687"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
user := msgraphsdk.NewTeamworkUserIdentity()
requestBody.SetUser(user)
id := "d864e79f-a516-4d0f-9fee-0eeb4d61fdc2"
user.SetId(&id)
tenantId := "2a690434-97d9-4eed-83a6-f5f13600199a"
requestBody.SetTenantId(&tenantId)
lastMessageReadDateTime, err := time.Parse(time.RFC3339, "2021-05-27T22:13:01.577Z")
requestBody.SetLastMessageReadDateTime(&lastMessageReadDateTime)
options := &msgraphsdk.MarkChatUnreadForUserRequestBuilderPostOptions{
    Body: requestBody,
}
chatId := "chat-id"
graphClient.ChatsById(&chatId).MarkChatUnreadForUser(chat-id).Post(options)


```