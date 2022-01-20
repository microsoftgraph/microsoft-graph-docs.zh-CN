---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 96076d4f3639b45eff5d99ce1e2f68a2443d2616
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62109293"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    PolicyViolation = @{
        PolicyTip = @{
            GeneralText = "This item has been blocked by the administrator."
            ComplianceUrl = "https://contoso.com/dlp-policy-page"
            MatchedConditionDescriptions = @(
                "Credit Card Number"
            )
        }
        VerdictDetails = "AllowOverrideWithoutJustification,AllowFalsePositiveOverride"
        DlpAction = "BlockAccess"
    }
}

Update-MgTeamChannelMessage -TeamId $teamId -ChannelId $channelId -ChatMessageId $chatMessageId -BodyParameter $params

```