---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 853621722bff5e5471c5111286e3f0a26cd0e575
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335848"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    TenantId = "3d0f5dec-5d3d-455c-8016-e2af1ae4d31a"
    B2bDirectConnectOutbound = @{
        UsersAndGroups = @{
            AccessType = "blocked"
            Targets = @(
                @{
                    Target = "6f546279-4da5-4b53-a095-09ea0cef9971"
                    TargetType = "group"
                }
            )
        }
    }
    B2bDirectConnectInbound = @{
        Applications = @{
            AccessType = "allowed"
            Targets = @(
                @{
                    Target = "Office365"
                    TargetType = "application"
                }
            )
        }
    }
}

New-MgPolicyCrossTenantAccessPolicyPartner -BodyParameter $params

```