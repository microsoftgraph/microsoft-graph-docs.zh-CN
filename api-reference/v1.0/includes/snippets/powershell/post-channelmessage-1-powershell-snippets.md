---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 325ddd235d1b1f0089648ea4f49799aaead6128e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62104943"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    Body = @{
        Content = "Hello World"
    }
}

New-MgTeamChannelMessage -TeamId $teamId -ChannelId $channelId -BodyParameter $params

```