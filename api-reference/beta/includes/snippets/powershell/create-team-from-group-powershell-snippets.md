---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 341cc87219af4b92ad0aba395ad505651d7fe88a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62102347"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    "Template@odata.bind" = "https://graph.microsoft.com/beta/teamsTemplates('standard')"
    "Group@odata.bind" = "https://graph.microsoft.com/beta/groups('71392b2f-1765-406e-86af-5907d9bdb2ab')"
}

New-MgTeam -BodyParameter $params

```