---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5753ca7cb3b03b41eebe06c2ca4b412259f621a9
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62339901"
---
```powershell

Import-Module Microsoft.Graph.Groups

$params = @{
    AddLicenses = @(
        @{
            DisabledPlans = @(
                "113feb6c-3fe4-4440-bddc-54d774bf0318"
                "14ab5db5-e6c4-4b20-b4bc-13e36fd2227f"
            )
            SkuId = "b05e124f-c7cc-45a0-a6aa-8cf78c946968"
        }
        @{
            DisabledPlans = @(
                "a413a9ff-720c-4822-98ef-2f37c2a21f4c"
            )
            SkuId = "c7df2760-2c81-4ef7-b578-5b5392b571df"
        }
    )
    RemoveLicenses = @(
    )
}

Set-MgGroupLicense -GroupId $groupId -BodyParameter $params

```