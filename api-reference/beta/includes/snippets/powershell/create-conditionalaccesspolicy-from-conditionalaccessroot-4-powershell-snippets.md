---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 50161a58ca23ce58d01241ac48e28d783238e54c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62135627"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    DisplayName = "Require MFA to EXO from non-complaint devices."
    State = "enabled"
    Conditions = @{
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
        Devices = @{
            IncludeDevices = @(
                "All"
            )
            ExcludeDevices = @(
                "Compliant"
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