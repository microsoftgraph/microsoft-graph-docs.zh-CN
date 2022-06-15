---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b3d41c32e6f16428851505c1c8944b32a48dbc3
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098808"
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
emailAddress := msgraphsdk.NewEmailAddress()
    SetEmailAddress(emailAddress)
name := "Alex Wilbur"
    emailAddress.SetName(&name)
address := "AlexW@contoso.onmicrosoft.com"
    emailAddress.SetAddress(&address)
}
stopProcessingRules := true
actions.SetStopProcessingRules(&stopProcessingRules)
mailFolderId := "mailFolder-id"
result, err := graphClient.Me().MailFoldersById(&mailFolderId).MessageRules().Post(requestBody)


```