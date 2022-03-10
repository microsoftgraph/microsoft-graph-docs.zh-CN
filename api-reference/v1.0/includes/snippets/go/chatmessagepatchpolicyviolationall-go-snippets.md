---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 660e012884ee67d4ad3276a215c943d3754879aa
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412461"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewChatMessage()
policyViolation := msgraphsdk.NewChatMessagePolicyViolation()
requestBody.SetPolicyViolation(policyViolation)
policyTip := msgraphsdk.NewChatMessagePolicyViolationPolicyTip()
policyViolation.SetPolicyTip(policyTip)
generalText := "This item has been blocked by the administrator."
policyTip.SetGeneralText(&generalText)
complianceUrl := "https://contoso.com/dlp-policy-page"
policyTip.SetComplianceUrl(&complianceUrl)
policyTip.SetMatchedConditionDescriptions( []String {
    "Credit Card Number",
}
verdictDetails := "AllowOverrideWithoutJustification,AllowFalsePositiveOverride"
policyViolation.SetVerdictDetails(&verdictDetails)
dlpAction := "BlockAccess"
policyViolation.SetDlpAction(&dlpAction)
options := &msgraphsdk.ChatMessageRequestBuilderPatchOptions{
    Body: requestBody,
}
teamId := "team-id"
channelId := "channel-id"
chatMessageId := "chatMessage-id"
result, err := graphClient.TeamsById(&teamId).ChannelsById(&channelId).MessagesById(&chatMessageId).Patch(options)


```