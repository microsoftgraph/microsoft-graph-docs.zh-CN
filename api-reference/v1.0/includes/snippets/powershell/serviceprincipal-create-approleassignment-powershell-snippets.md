---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 24c7a3d3f2c8a2e8580e58a335d3b4254c8d08b6
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62121902"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    PrincipalId = "9028d19c-26a9-4809-8e3f-20ff73e2d75e"
    ResourceId = "8fce32da-1246-437b-99cd-76d1d4677bd5"
    AppRoleId = "498476ce-e0fe-48b0-b801-37ba7e2685c6"
}

New-MgServicePrincipalAppRoleAssignment -ServicePrincipalId $servicePrincipalId -BodyParameter $params

```