---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f9fbbb16201fa8b748daf648412893228733b01f
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61099036"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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