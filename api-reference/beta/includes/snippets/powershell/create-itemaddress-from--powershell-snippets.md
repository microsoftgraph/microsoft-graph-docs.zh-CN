---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c16ef3bc158436a3adb3ce72bad5bec4810a743a
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351627"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    DisplayName = "Home"
    Detail = @{
        Type = "home"
        PostOfficeBox = $null
        Street = "221B Baker Street"
        City = "London"
        State = $null
        CountryOrRegion = "United Kingdom"
        PostalCode = "E14 3TD"
    }
}

# A UPN can also be used as -UserId.
New-MgUserProfileAddress -UserId $userId -BodyParameter $params

```