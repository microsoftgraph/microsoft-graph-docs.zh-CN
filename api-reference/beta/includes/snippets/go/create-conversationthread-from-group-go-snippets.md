---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ff79a95a93d032043f6e5cc08a568946a26f3526
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098795"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewConversationThread()
topic := "New Conversation Thread Topic"
requestBody.SetTopic(&topic)
requestBody.SetPosts( []Post {
    msgraphsdk.NewPost(),
body := msgraphsdk.NewItemBody()
    SetBody(body)
contentType := "html"
    body.SetContentType(&contentType)
content := "this is body content"
    body.SetContent(&content)
    SetNewParticipants( []Recipient {
        msgraphsdk.NewRecipient(),
        SetAdditionalData(map[string]interface{}{
        }
    }
}
groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).Threads().Post(requestBody)


```