---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 87767e647897cb07549b1e8cdcade1353a89c229
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62129036"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgTeamChannelMember -TeamId $teamId -ChannelId $channelId

```