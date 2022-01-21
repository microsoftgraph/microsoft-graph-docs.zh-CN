---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 01d819fae343513c307390c442b9796e9c910d1c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62125990"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    DisplayName = "UpdateChannelModeration"
    Description = "Update channel moderation."
    ModerationSettings = @{
        UserNewMessageRestriction = "moderators"
        ReplyRestriction = "everyone"
        AllowNewMessageFromBots = $true
        AllowNewMessageFromConnectors = $true
    }
}

Update-MgTeamChannel -TeamId $teamId -ChannelId $channelId -BodyParameter $params

```