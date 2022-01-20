---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cf9ada0382fcd5231029526fa78a4c80f357d922
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62118088"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgTeamTagMember -TeamId $teamId -TeamworkTagId $teamworkTagId -TeamworkTagMemberId $teamworkTagMemberId

```