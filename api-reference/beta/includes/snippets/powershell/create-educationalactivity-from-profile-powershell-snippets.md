---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 37d9d5f7c4b2137000bee8569f8a3e0db7343a37
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350687"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    CompletionMonthYear = "Date"
    EndMonthYear = "Date"
    Institution = @{
        Description = $null
        DisplayName = "Colorado State University"
        Location = @{
            Type = "business"
            PostOfficeBox = $null
            Street = "12000 E Prospect Rd"
            City = "Fort Collins"
            State = "Colorado"
            CountryOrRegion = "USA"
            PostalCode = "80525"
        }
        WebUrl = "https://www.colostate.edu"
    }
    Program = @{
        Abbreviation = "MBA"
        Activities = $null
        Awards = $null
        Description = "Master of Business Administration with a major in Entreprenuership and Finance."
        DisplayName = "Master of Business Administration"
        FieldsOfStudy = $null
        Grade = "3.9"
        Notes = $null
        WebUrl = "https://biz.colostate.edu"
    }
    StartMonthYear = "Date"
}

# A UPN can also be used as -UserId.
New-MgUserProfileEducationalActivity -UserId $userId -BodyParameter $params

```