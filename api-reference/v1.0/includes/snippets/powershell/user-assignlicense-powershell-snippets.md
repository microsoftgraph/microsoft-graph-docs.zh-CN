---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 338d6bb704de4a234aaa5bf2b270df46966f0455
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336821"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    AddLicenses = @(
        @{
            DisabledPlans = @(
                "11b0131d-43c8-4bbb-b2c8-e80f9a50834a"
            )
            SkuId = "45715bb8-13f9-4bf6-927f-ef96c102d394"
        }
    )
    RemoveLicenses = @(
        "bea13e0c-3828-4daa-a392-28af7ff61a0f"
    )
}

# A UPN can also be used as -UserId.
Set-MgUserLicense -UserId $userId -BodyParameter $params

```