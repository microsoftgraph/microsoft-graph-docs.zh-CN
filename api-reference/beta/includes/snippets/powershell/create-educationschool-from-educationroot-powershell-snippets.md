---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 889d2ea5e7e7c9324cafe7c3947929fedf745078
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62120721"
---
```powershell

Import-Module Microsoft.Graph.Education

$params = @{
    DisplayName = "Fabrikam High School"
    Description = "Magnate school for the arts. Los Angeles School District"
    ExternalSource = "String"
    PrincipalEmail = "AmyR@fabrikam.com"
    PrincipalName = "Amy Roebuck"
    ExternalPrincipalId = "14007"
    HighestGrade = "12"
    LowestGrade = "9"
    SchoolNumber = "10002"
    Address = @{
        City = "Los Angeles"
        CountryOrRegion = "United States"
        PostalCode = "98055"
        State = "CA"
        Street = "12345 Main St."
    }
    ExternalId = "10002"
    Phone = "+1 (253) 555-0102"
}

New-MgEducationSchool -BodyParameter $params

```