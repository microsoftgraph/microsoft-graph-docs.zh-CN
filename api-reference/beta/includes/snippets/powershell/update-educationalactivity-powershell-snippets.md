---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1ab85880296e8e8b9056bff3b5b009d26be684cf
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62123716"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    Institution = @{
        Location = @{
            Type = "business"
            PostOfficeBox = $null
            Street = "12000 E Prospect Rd"
            City = "Fort Collins"
            State = "Colorado"
            CountryOrRegion = "USA"
            PostalCode = "80525"
        }
    }
}

Update-MgUserProfileEducationalActivity -UserId $userId -EducationalActivityId $educationalActivityId -BodyParameter $params

```