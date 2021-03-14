---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 839dc231f398ecf00fd87367ca103d37a3eaa7b1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779143"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chatMessage = new ChatMessage
{
    PolicyViolation = new ChatMessagePolicyViolation
    {
        PolicyTip = new ChatMessagePolicyViolationPolicyTip
        {
            GeneralText = "This item has been blocked by the administrator.",
            ComplianceUrl = "https://contoso.com/dlp-policy-page",
            MatchedConditionDescriptions = new List<String>()
            {
                "Credit Card Number"
            }
        },
        VerdictDetails = ChatMessagePolicyViolationVerdictDetailsTypes.AllowFalsePositiveOverride | ChatMessagePolicyViolationVerdictDetailsTypes.AllowOverrideWithoutJustification,
        DlpAction = ChatMessagePolicyViolationDlpActionTypes.BlockAccess
    }
};

await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Messages["{chatMessage-id}"]
    .Request()
    .UpdateAsync(chatMessage);

```