---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 507073cf3e2fcbfa415ca065429f8de3c95d640b
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62343151"
---
```powershell

Import-Module Microsoft.Graph.Teams

New-MgTeamChannelEmail -TeamId $teamId -ChannelId $channelId

```