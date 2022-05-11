---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 20e2a4809da84ca930e9f7f7b2b84072ae4f631f
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315019"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgTeamChannelMessage -TeamId $teamId -ChannelId $channelId -Top 3 

```