---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6e7adc0ac4131e5ff2623a184b17eb055c85559f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62129049"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgTeamChannelMessage -TeamId $teamId -ChannelId $channelId

```