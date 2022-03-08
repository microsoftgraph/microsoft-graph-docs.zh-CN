---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7c784d9dd494f569284a385a514d18ff25d6bbe3
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63340034"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    AddLicenses = @(
    )
    RemoveLicenses = @(
        "f30db892-07e9-47e9-837c-80727f46fd3d"
        "84a661c4-e949-4bd2-a560-ed7766fcaf2b"
    )
}

# A UPN can also be used as -UserId.
Set-MgUserLicense -UserId $userId -BodyParameter $params

```