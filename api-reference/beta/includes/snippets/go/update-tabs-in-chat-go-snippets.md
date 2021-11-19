---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3abb4f66cae6db1342506e87f062152f07a1b2b5
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61098709"
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
graphClient.ChatsById(&chatId).TabsById(&teamsTabId).Patch(options)


```