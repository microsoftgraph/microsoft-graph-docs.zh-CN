---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e81189b2718a190159f59b3ba90909414f7b22df
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62129351"
---
```powershell

Import-Module Microsoft.Graph.Teams

Remove-MgTeamTagMember -TeamId $teamId -TeamworkTagId $teamworkTagId -TeamworkTagMemberId $teamworkTagMemberId

```