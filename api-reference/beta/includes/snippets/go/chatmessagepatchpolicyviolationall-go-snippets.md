---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 15fbfbc113ff2b8e404b281e5ef35443ef88b4bd
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328453"
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
teamId := "team-id"
channelId := "channel-id"
chatMessageId := "chatMessage-id"
graphClient.TeamsById(&teamId).ChannelsById(&channelId).MessagesById(&chatMessageId).Patch(requestBody)


```