---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 729c35dfbf28fa98ecbe85218e6db3311bac330d
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412673"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewMessageRule()
displayName := "Important from partner"
requestBody.SetDisplayName(&displayName)
actions := msgraphsdk.NewMessageRuleActions()
requestBody.SetActions(actions)
markImportance := "high"
actions.SetMarkImportance(&markImportance)
options := &msgraphsdk.MessageRuleRequestBuilderPatchOptions{
    Body: requestBody,
}
mailFolderId := "mailFolder-id"
messageRuleId := "messageRule-id"
result, err := graphClient.Me().MailFoldersById(&mailFolderId).MessageRulesById(&messageRuleId).Patch(options)


```