---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f4ccbf3e1c28aa8c1645aae503dd51c1d20284c9
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60975845"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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