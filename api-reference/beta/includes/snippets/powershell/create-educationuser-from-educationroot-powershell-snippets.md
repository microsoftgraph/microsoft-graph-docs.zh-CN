---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c918cbdecb85066e42f1b69eee6b17060adba21b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62106233"
---
```powershell

Import-Module Microsoft.Graph.Education

$params = @{
    DisplayName = "Dion Matheson"
    GivenName = "Dion"
    MiddleName = $null
    Surname = "Matheson"
    Mail = "DionM@contoso.com"
    MobilePhone = "+1 (253) 555-0101"
    CreatedBy = @{
        User = @{
            DisplayName = "Susana Rocha"
            Id = "14012"
        }
    }
    ExternalSource = "sis"
    MailingAddress = @{
        City = "Los Angeles"
        CountryOrRegion = "United States"
        PostalCode = "98055"
        State = "CA"
        Street = "12345 Main St."
    }
    PrimaryRole = "student"
    ResidenceAddress = @{
        City = "Los Angeles"
        CountryOrRegion = "United States"
        PostalCode = "98055"
        State = "CA"
        Street = "12345 Main St."
    }
}

New-MgEducationUser -BodyParameter $params

```