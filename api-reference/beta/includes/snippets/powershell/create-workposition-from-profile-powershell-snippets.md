---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d9252e00c0cd5d17fa79cc33282ef8b704857653
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349721"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    Detail = @{
        Company = @{
            DisplayName = "Adventureworks Ltd."
            Department = "Consulting"
            OfficeLocation = "AW23/344"
            Address = @{
                Type = "business"
                Street = "123 Patriachy Ponds"
                City = "Moscow"
                CountryOrRegion = "Russian Federation"
                PostalCode = "RU-34621"
            }
            WebUrl = "https://www.adventureworks.com"
        }
        JobTitle = "Senior Product Branding Manager II"
        Role = "consulting"
    }
    IsCurrent = $true
}

# A UPN can also be used as -UserId.
New-MgUserProfilePosition -UserId $userId -BodyParameter $params

```