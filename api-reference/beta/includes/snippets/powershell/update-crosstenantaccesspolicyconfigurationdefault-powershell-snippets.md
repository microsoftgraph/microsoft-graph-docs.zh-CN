---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ff1159abffc497944f7445a265f3759e802e94d
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335547"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    B2bCollaborationOutbound = @{
        UsersAndGroups = @{
            AccessType = "blocked"
            Targets = @(
                @{
                    Target = "0be493dc-cb56-4a53-936f-9cf64410b8b0"
                    TargetType = "group"
                }
            )
        }
        Applications = @{
            AccessType = "blocked"
            Targets = @(
                @{
                    Target = "AllApplications"
                    TargetType = "application"
                }
            )
        }
    }
}

Update-MgPolicyCrossTenantAccessPolicyDefault -BodyParameter $params

```