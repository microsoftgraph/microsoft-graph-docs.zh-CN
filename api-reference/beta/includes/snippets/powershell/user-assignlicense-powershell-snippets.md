---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e9edccc447311dab46050eba2f63096aa2eec055
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63340027"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    AddLicenses = @(
        @{
            DisabledPlans = @(
                "8a256a2b-b617-496d-b51b-e76466e88db0"
            )
            SkuId = "84a661c4-e949-4bd2-a560-ed7766fcaf2b"
        }
        @{
            DisabledPlans = @(
            )
            SkuId = "f30db892-07e9-47e9-837c-80727f46fd3d"
        }
    )
    RemoveLicenses = @(
    )
}

# A UPN can also be used as -UserId.
Set-MgUserLicense -UserId $userId -BodyParameter $params

```