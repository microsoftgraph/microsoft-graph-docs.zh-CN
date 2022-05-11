---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b18d39c160ebaefa8b8bf7556831e79af76a0f5
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327016"
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
groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).Threads().Post(requestBody)


```