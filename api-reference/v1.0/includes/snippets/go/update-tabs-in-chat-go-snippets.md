---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1856c52690b402410e4bacd80a38feace6eef4c6
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411720"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTeamsTab()
displayName := "My Contoso Tab - updated again"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.TeamsTabRequestBuilderPatchOptions{
    Body: requestBody,
}
chatId := "chat-id"
teamsTabId := "teamsTab-id"
result, err := graphClient.ChatsById(&chatId).TabsById(&teamsTabId).Patch(options)


```