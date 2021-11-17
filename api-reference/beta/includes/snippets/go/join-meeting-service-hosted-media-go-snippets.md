---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a330296f40d5958ce9501c11f7734ff602d162d
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60983140"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewCall()
callbackUri := "https://bot.contoso.com/callback"
requestBody.SetCallbackUri(&callbackUri)
requestBody.SetRequestedModalities( []Modality {
    "audio",
}
mediaConfig := msgraphsdk.NewMediaConfig()
requestBody.SetMediaConfig(mediaConfig)
mediaConfig.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig",
    "preFetchMedia":  []Object {
    }
}
chatInfo := msgraphsdk.NewChatInfo()
requestBody.SetChatInfo(chatInfo)
threadId := "19:meeting_Win6Ydo4wsMijFjZS00ZGVjLTk5MGUtOTRjNWY2NmNkYTFm@thread.v2"
chatInfo.SetThreadId(&threadId)
messageId := "0"
chatInfo.SetMessageId(&messageId)
chatInfo.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.chatInfo",
}
meetingInfo := msgraphsdk.NewMeetingInfo()
requestBody.SetMeetingInfo(meetingInfo)
allowConversationWithoutHost := true
meetingInfo.SetAllowConversationWithoutHost(&allowConversationWithoutHost)
meetingInfo.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.organizerMeetingInfo",
}
tenantId := "86dc81db-c112-4228-9222-63f3esaa1edb"
requestBody.SetTenantId(&tenantId)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.call",
}
options := &msgraphsdk.CallsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Communications().Calls().Post(options)


```