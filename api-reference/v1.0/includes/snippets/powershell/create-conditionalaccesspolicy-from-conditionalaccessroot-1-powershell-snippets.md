---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 08b9dc770ed6b00edd1f826a795dda1b5905c3bc
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62101458"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    DisplayName = "Access to EXO requires MFA"
    State = "enabled"
    Conditions = @{
        ClientAppTypes = @(
            "mobileAppsAndDesktopClients"
            "browser"
        )
        Applications = @{
            IncludeApplications = @(
                "00000002-0000-0ff1-ce00-000000000000"
            )
        }
        Users = @{
            IncludeGroups = @(
                "ba8e7ded-8b0f-4836-ba06-8ff1ecc5c8ba"
            )
        }
        Locations = @{
            IncludeLocations = @(
                "All"
            )
            ExcludeLocations = @(
                "AllTrusted"
            )
        }
    }
    GrantControls = @{
        Operator = "OR"
        BuiltInControls = @(
            "mfa"
        )
    }
}

New-MgIdentityConditionalAccessPolicy -BodyParameter $params

```