---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bd29e0e6a4fbe333180012fff3155c38eddddb18
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411686"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewChat()
topic := "Group chat title update"
requestBody.SetTopic(&topic)
options := &msgraphsdk.ChatRequestBuilderPatchOptions{
    Body: requestBody,
}
chatId := "chat-id"
result, err := graphClient.ChatsById(&chatId).Patch(options)


```