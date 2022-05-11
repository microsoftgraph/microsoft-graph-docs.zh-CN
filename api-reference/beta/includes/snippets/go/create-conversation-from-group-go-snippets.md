---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ddd7adf931136b1800a57084d814a2faa9dc3c6
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327981"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewConversation()
topic := "New head count"
requestBody.SetTopic(&topic)
requestBody.SetThreads( []ConversationThread {
    msgraphsdk.NewConversationThread(),
    SetAdditionalData(map[string]interface{}{
        "posts":  []Object {
        }
    }
}
groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).Conversations().Post(requestBody)


```