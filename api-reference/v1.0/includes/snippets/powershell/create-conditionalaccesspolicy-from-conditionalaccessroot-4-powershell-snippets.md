---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cb21ec2cfef0dd3e2f6fda47213226e047b20c8f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62101460"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    DisplayName = "Require MFA to EXO from non-compliant devices."
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