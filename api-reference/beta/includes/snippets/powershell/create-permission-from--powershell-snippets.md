---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a3a75d01d86dd2a9fd84ac34a766ea8e37362b55
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62111710"
---
```powershell

Import-Module Microsoft.Graph.Sites

$params = @{
    Roles = @(
        "write"
    )
    GrantedToIdentities = @(
        @{
            Application = @{
                Id = "89ea5c94-7736-4e25-95ad-3fa95f62b66e"
                DisplayName = "Contoso Time Manager App"
            }
        }
    )
}

New-MgSitePermission -SiteId $siteId -BodyParameter $params

```