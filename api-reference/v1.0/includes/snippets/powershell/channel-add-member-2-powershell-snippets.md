---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ef47aa34134cd9ddced76debd7573c71e3dca1fe
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62124942"
---
```powershell

Import-Module Microsoft.Graph.Teams

New-MgTeamChannelMember -TeamId $teamId -ChannelId $channelId

```