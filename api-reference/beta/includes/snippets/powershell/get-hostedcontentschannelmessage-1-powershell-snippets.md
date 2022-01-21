---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba5a0af26977ebe010e2e84f6893e3ed9adced56
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62123975"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgTeamChannelMessageHostedContent -TeamId $teamId -ChannelId $channelId -ChatMessageId $chatMessageId

```