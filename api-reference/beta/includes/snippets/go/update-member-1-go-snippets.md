---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2bb8df3f8767629cd9e21b393f118426e994e6db
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325953"
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
teamId := "team-id"
channelId := "channel-id"
conversationMemberId := "conversationMember-id"
graphClient.TeamsById(&teamId).ChannelsById(&channelId).MembersById(&conversationMemberId).Patch(requestBody)


```