---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4418dc0b7464d2a0938bd142b3268eb33a87861b
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61087965"
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
graphClient.TeamsById(&teamId).ChannelsById(&channelId).MessagesById(&chatMessageId).Patch(options)


```