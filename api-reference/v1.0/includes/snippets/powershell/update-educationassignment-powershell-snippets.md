---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c00e37687231c6056739b0a3a184a5d927c6ed6e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62092359"
---
```powershell

Import-Module Microsoft.Graph.Education

$params = @{
    DisplayName = "Reading and review test 09.03 #5"
    Instructions = @{
        ContentType = "text"
        Content = "Read chapter 5 and write your review"
    }
    DueDateTime = [System.DateTime]::Parse("2021-09-10T00:00:00Z")
    AddedStudentAction = "none"
}

Update-MgEducationClassAssignment -EducationClassId $educationClassId -EducationAssignmentId $educationAssignmentId -BodyParameter $params

```