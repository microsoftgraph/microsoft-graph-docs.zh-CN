---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d36dea1c6ef5870bac71cb90aaf16c8b74c0932c
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62344337"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgTeamChannelMessageDelta -TeamId $teamId -ChannelId $channelId -Skiptoken "8UusBixEHS9UUau6uGcryrA6FpnWwMJbuTYILM1PArHxnZzDVcsHQrijNzCyIVeEauMQsKUfMhNjLWFs1o4sBS_LofJ7xMftZUfec_pijuT6cAk5ugcWCca9RCjK7iVj.DKZ9w4bX9vCR7Sj9P0_qxjLAAPiEZgxlOxxmCLMzHJ4" 

```