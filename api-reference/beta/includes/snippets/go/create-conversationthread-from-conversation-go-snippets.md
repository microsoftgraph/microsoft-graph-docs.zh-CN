---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8bb2a3f4bdde01435ada3f120e4e8da3338fa39e
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60987132"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewConversationThread()
topic := "Take your wellness days and rest"
requestBody.SetTopic(&topic)
requestBody.SetPosts( []Post {
    msgraphsdk.NewPost(),
    SetAdditionalData(map[string]interface{}{
    }
}
options := &msgraphsdk.ThreadsRequestBuilderPostOptions{
    Body: requestBody,
}
groupId := "group-id"
conversationId := "conversation-id"
result, err := graphClient.GroupsById(&groupId).ConversationsById(&conversationId).Threads().Post(options)


```