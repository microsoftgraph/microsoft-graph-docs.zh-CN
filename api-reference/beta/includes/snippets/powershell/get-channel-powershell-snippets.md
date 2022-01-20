---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a6fb48739841aacc53a0148a0053cd771ed44461
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62119347"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgTeamChannel -TeamId $teamId -ChannelId $channelId

```