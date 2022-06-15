---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ea77ef0aa63253286a05eff36946ce3faecf6302
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098718"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewConversation()
topic := "Take your wellness days and rest"
requestBody.SetTopic(&topic)
requestBody.SetThreads( []ConversationThread {
    msgraphsdk.NewConversationThread(),
    SetPosts( []Post {
        msgraphsdk.NewPost(),
body := msgraphsdk.NewItemBody()
        SetBody(body)
contentType := "html"
        body.SetContentType(&contentType)
content := "Contoso cares about you: Rest and Recharge"
        body.SetContent(&content)
        SetNewParticipants( []Recipient {
            msgraphsdk.NewRecipient(),
            SetAdditionalData(map[string]interface{}{
            }
        }
    }
}
groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).Conversations().Post(requestBody)


```