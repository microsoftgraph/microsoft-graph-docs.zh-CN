---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 13eaab2768c562202a2008e776e18c4b33adbd93
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62087692"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    "Template@odata.bind" = "https://graph.microsoft.com/v1.0/teamsTemplates('educationClass')"
    DisplayName = "My Class Team"
    Description = "My Class Team’s Description"
}

New-MgTeam -BodyParameter $params

```