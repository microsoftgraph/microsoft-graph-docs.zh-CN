---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b59106f3bb1a99e149e5154615b0c6cea506aee8
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62135273"
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

New-MgUserProfileEducationalActivity -UserId $userId -BodyParameter $params

```