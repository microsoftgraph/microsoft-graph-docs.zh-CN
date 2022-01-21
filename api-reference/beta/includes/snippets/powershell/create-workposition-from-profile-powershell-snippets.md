---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 13a78d91e146c0cc7b4511b0aedd39d25388d3a7
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62135245"
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

New-MgUserProfilePosition -UserId $userId -BodyParameter $params

```