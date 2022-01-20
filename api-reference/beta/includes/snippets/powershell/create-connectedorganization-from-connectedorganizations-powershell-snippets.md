---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f1365fcf232e569cc5920d5c45804fe400997c54
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62129827"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    DisplayName = "Connected organization name"
    Description = "Connected organization description"
    IdentitySources = @(
        @{
            "@odata.type" = "#microsoft.graph.domainIdentitySource"
            DomainName = "example.com"
            DisplayName = "example.com"
        }
    )
    State = "proposed"
}

New-MgEntitlementManagementConnectedOrganization -BodyParameter $params

```