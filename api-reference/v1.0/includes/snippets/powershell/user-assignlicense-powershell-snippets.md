---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ef8cbc25f66aecaa832e7f8e69ea05635454f42
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62344711"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    AddLicenses = @(
        @{
            DisabledPlans = @(
                "11b0131d-43c8-4bbb-b2c8-e80f9a50834a"
            )
            SkuId = "guid"
        }
    )
    RemoveLicenses = @(
        "bea13e0c-3828-4daa-a392-28af7ff61a0f"
    )
}

# A UPN can also be used as -UserId.
Set-MgUserLicense -UserId $userId -BodyParameter $params

```