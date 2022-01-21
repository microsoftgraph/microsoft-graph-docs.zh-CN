---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c25b228e60f83ae295c7714b1c0e733187a51eb
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62136246"
---
```powershell

Import-Module Microsoft.Graph.Education

$params = @{
    "@odata.type" = "#microsoft.graph.educationSchool"
    DisplayName = "String"
    Description = "String"
    ExternalSource = "String"
    ExternalSourceDetail = "String"
    PrincipalEmail = "String"
    PrincipalName = "String"
    ExternalPrincipalId = "String"
    LowestGrade = "String"
    HighestGrade = "String"
    SchoolNumber = "String"
    ExternalId = "String"
    Phone = "String"
    Fax = "String"
    CreatedBy = @{
        "@odata.type" = "microsoft.graph.identitySet"
    }
    Address = @{
        "@odata.type" = "microsoft.graph.physicalAddress"
    }
}

New-MgEducationSchool -BodyParameter $params

```