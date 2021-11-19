---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fba549c4a89fe8b0e8b3920454ff178f18178975
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090743"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewConversationMember()
visibleHistoryStartDateTime, err := time.Parse(time.RFC3339, "0001-01-01T00:00:00Z")
requestBody.SetVisibleHistoryStartDateTime(&visibleHistoryStartDateTime)
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