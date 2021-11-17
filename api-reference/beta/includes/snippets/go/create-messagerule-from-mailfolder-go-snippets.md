---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 976fcbfa3280869c2c8d49004deed005bb4c406b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61034235"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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