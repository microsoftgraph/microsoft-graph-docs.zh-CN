---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 42a18723a2f25690a86da24579fb5d0a7ccf8572
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223249"
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

await graphClient.Teams["e1234567-e123-4276-55555-6232b0e3a89a"].Channels["a7654321-e321-0000-0000-123b0e3a00a"].Messages["19:a21b0b0c05194ebc9e30000000000f61@thread.skype"]
    .Request()
    .UpdateAsync(chatMessage);

```