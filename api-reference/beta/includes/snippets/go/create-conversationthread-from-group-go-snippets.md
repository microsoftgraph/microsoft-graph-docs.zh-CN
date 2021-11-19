---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 512e4fe2e65fe4388adf6d8388ff93ba01fe9425
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088930"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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