---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3c51bf27b6c427c1b28af5333a8b109e78d2cb74
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315023"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgTeamChannelMessage -TeamId $teamId -ChannelId $channelId -Top 1 -ExpandProperty "replies" 

```