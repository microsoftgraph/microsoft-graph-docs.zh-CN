---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f25c792f34518223b60e3d3722b3033c6f11247
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60974962"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewConversationThread()
topic := "New Conversation Thread Topic"
requestBody.SetTopic(&topic)
requestBody.SetPosts( []Post {
    msgraphsdk.NewPost(),
    SetAdditionalData(map[string]interface{}{
        "newParticipants":  []Object {
        }
    }
}
options := &msgraphsdk.ThreadsRequestBuilderPostOptions{
    Body: requestBody,
}
groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).Threads().Post(options)


```