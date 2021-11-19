---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1270bc16e5cf09acf89d7d58e5bdfd238ef338f9
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61084472"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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