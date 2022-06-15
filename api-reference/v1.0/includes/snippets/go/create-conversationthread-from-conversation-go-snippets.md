---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d94ff07c011ac58f2ce5affd2b9680d35a320d72
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098722"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewConversationThread()
topic := "Take your wellness days and rest"
requestBody.SetTopic(&topic)
requestBody.SetPosts( []Post {
    msgraphsdk.NewPost(),
body := msgraphsdk.NewItemBody()
    SetBody(body)
contentType := "html"
    body.SetContentType(&contentType)
content := "Waiting for the summer holidays."
    body.SetContent(&content)
}
groupId := "group-id"
conversationId := "conversation-id"
result, err := graphClient.GroupsById(&groupId).ConversationsById(&conversationId).Threads().Post(requestBody)


```