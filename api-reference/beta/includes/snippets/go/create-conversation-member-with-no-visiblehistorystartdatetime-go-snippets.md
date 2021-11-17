---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae2759e1c3dbe3a756197780c27c3630aa091765
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61005826"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewConversationMember()
requestBody.SetRoles( []String {
    "owner",
}
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
    "user@odata.bind": "https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5",
}
options := &msgraphsdk.MembersRequestBuilderPostOptions{
    Body: requestBody,
}
chatId := "chat-id"
result, err := graphClient.ChatsById(&chatId).Members().Post(options)


```