---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 186de5fdc62a3b9365c1c3ff6e3796cfddbc67bd
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098696"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewConversation()
topic := "New head count"
requestBody.SetTopic(&topic)
requestBody.SetThreads( []ConversationThread {
    msgraphsdk.NewConversationThread(),
    SetPosts( []Post {
        msgraphsdk.NewPost(),
body := msgraphsdk.NewItemBody()
        SetBody(body)
contentType := "html"
        body.SetContentType(&contentType)
content := "The confirmation will come by the end of the week."
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