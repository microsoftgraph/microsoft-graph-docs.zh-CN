---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8e7a920d633d1a6abcab904b874261f3a2e17ae9
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61095293"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewConversationMember()
requestBody.SetRoles( []String {
    "owner",
}
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
}
options := &msgraphsdk.ConversationMemberRequestBuilderPatchOptions{
    Body: requestBody,
}
teamId := "team-id"
channelId := "channel-id"
conversationMemberId := "conversationMember-id"
graphClient.TeamsById(&teamId).ChannelsById(&channelId).MembersById(&conversationMemberId).Patch(options)


```