---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dfb518422187b8db572dfc94ab08b3017af9a10e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61093215"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewMessageRule()
displayName := "From partner"
requestBody.SetDisplayName(&displayName)
sequence := int32(2)
requestBody.SetSequence(&sequence)
isEnabled := true
requestBody.SetIsEnabled(&isEnabled)
conditions := msgraphsdk.NewMessageRulePredicates()
requestBody.SetConditions(conditions)
conditions.SetSenderContains( []String {
    "adele",
}
actions := msgraphsdk.NewMessageRuleActions()
requestBody.SetActions(actions)
actions.SetForwardTo( []Recipient {
    msgraphsdk.NewRecipient(),
    SetAdditionalData(map[string]interface{}{
    }
}
stopProcessingRules := true
actions.SetStopProcessingRules(&stopProcessingRules)
options := &msgraphsdk.MessageRulesRequestBuilderPostOptions{
    Body: requestBody,
}
mailFolderId := "mailFolder-id"
result, err := graphClient.Me().MailFoldersById(&mailFolderId).MessageRules().Post(options)


```