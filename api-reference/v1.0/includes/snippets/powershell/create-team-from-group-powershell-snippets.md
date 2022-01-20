---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f83cfc0bbc2b978350e1162035439f1d3861b8b8
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62087689"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    "Template@odata.bind" = "https://graph.microsoft.com/v1.0/teamsTemplates('standard')"
    "Group@odata.bind" = "https://graph.microsoft.com/v1.0/groups('71392b2f-1765-406e-86af-5907d9bdb2ab')"
}

New-MgTeam -BodyParameter $params

```