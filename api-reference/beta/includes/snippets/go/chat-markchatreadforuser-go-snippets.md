---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d67f0594a4718a42971111336f57d0746e63355c
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60994558"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
user := msgraphsdk.NewTeamworkUserIdentity()
requestBody.SetUser(user)
user.SetAdditionalData(map[string]interface{}{
    "id": "d864e79f-a516-4d0f-9fee-0eeb4d61fdc2",
}
tenantId := "2a690434-97d9-4eed-83a6-f5f13600199a"
requestBody.SetTenantId(&tenantId)
options := &msgraphsdk.MarkChatReadForUserRequestBuilderPostOptions{
    Body: requestBody,
}
chatId := "chat-id"
graphClient.ChatsById(&chatId).MarkChatReadForUser().Post(options)


```