---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aec812b4363d8a0f288311033eb05773c7ecbf35
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326829"
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
groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).Conversations().Post(requestBody)


```