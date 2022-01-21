---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 765b585c5e74e08e66518756e11adf8c14bde172
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62131566"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    DisplayName = "TestChannelModeration"
    Description = "Test channel moderation."
    MembershipType = "standard"
    ModerationSettings = @{
        UserNewMessageRestriction = "everyoneExceptGuests"
        ReplyRestriction = "everyone"
        AllowNewMessageFromBots = $true
        AllowNewMessageFromConnectors = $true
    }
}

New-MgTeamChannel -TeamId $teamId -BodyParameter $params

```