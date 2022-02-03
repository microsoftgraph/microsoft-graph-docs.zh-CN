---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d549f397c13600dddd2092a1660c30a58f2d3d1
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62344859"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    AddLicenses = @(
        @{
            DisabledPlans = @(
                "11b0131d-43c8-4bbb-b2c8-e80f9a50834a"
            )
            SkuId = "skuId-value-1"
        }
        @{
            DisabledPlans = @(
                "a571ebcc-fqe0-4ca2-8c8c-7a284fd6c235"
            )
            SkuId = "skuId-value-2"
        }
    )
    RemoveLicenses = @(
    )
}

# A UPN can also be used as -UserId.
Set-MgUserLicense -UserId $userId -BodyParameter $params

```