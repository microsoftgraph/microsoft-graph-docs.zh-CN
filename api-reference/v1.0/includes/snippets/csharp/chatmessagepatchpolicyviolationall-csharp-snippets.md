---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eeb86a24af3ca22123bd563a522ff589bd373d7c9bb851e9bf95f90dbe6dc0d4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409354"
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