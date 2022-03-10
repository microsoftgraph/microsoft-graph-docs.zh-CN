---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 08c32e1a7626ceef22f481341b5d45e1a24e2ed7
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411876"
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
result, err := graphClient.TeamsById(&teamId).ChannelsById(&channelId).MembersById(&conversationMemberId).Patch(options)


```