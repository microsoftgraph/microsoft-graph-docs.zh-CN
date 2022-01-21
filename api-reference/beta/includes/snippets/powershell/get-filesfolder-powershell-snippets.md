---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e561d91e234e9faf83584e493a9a1fe9e8762e74
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62128097"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgTeamChannelFileFolder -TeamId $teamId -ChannelId $channelId

```