---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e8ac2dd8af53589236d6b7e9a30020849a24a1b4
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61102175"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewConversationThread()
requestBody.SetAdditionalData(map[string]interface{}{
    "originalStartTimeZone": "originalStartTimeZone-value",
    "originalEndTimeZone": "originalEndTimeZone-value",
    "uid": "iCalUId-value",
    "reminderMinutesBeforeStart": ,
    "isReminderOn": true,
}
options := &msgraphsdk.ConversationThreadRequestBuilderPatchOptions{
    Body: requestBody,
}
groupId := "group-id"
conversationThreadId := "conversationThread-id"
graphClient.GroupsById(&groupId).ThreadsById(&conversationThreadId).Patch(options)


```