---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8cb24db22c8511ff352272c8ae015a68371375d1
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62130478"
---
```powershell

Import-Module Microsoft.Graph.Education

$params = @{
    DueDateTime = [System.DateTime]::Parse("2021-09-07T00:00:00Z")
    DisplayName = "Reading test 09.03 #4"
    Instructions = @{
        ContentType = "text"
        Content = "Read chapter 4"
    }
    Grading = @{
        "@odata.type" = "#microsoft.graph.educationAssignmentPointsGradeType"
        MaxPoints = 
    }
    AssignTo = @{
        "@odata.type" = "#microsoft.graph.educationAssignmentClassRecipient"
    }
    Status = "draft"
    AllowStudentsToAddResourcesToSubmission = $true
}

New-MgEducationClassAssignment -EducationClassId $educationClassId -BodyParameter $params

```