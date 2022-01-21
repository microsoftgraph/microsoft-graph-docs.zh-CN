---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4734b7aca78d4b489beca472f1fddf8c6102054f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62102349"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    "Template@odata.bind" = "https://graph.microsoft.com/beta/teamsTemplates('educationClass')"
    DisplayName = "My Class Team"
    Description = "My Class Team’s Description"
}

New-MgTeam -BodyParameter $params

```