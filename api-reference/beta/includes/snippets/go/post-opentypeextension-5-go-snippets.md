---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e1935413bbc72651e96638debbc24f6db5c9e83
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60986000"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewConversation()
topic := "Does anyone have a second?"
requestBody.SetTopic(&topic)
requestBody.SetThreads( []ConversationThread {
    msgraphsdk.NewConversationThread(),
    SetAdditionalData(map[string]interface{}{
        "Posts":  []Object {
        }
    }
}
options := &msgraphsdk.ConversationsRequestBuilderPostOptions{
    Body: requestBody,
}
groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).Conversations().Post(options)


```