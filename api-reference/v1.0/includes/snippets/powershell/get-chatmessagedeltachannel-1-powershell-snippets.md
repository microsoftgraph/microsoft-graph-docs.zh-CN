---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b9bc244978f3c2306d00f3c17764062fc95dc394
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62344339"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgTeamChannelMessageDelta -TeamId $teamId -ChannelId $channelId -Top 2 

```