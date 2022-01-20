---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b34795ae017fbc84a9e09750bf939ff308422404
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62097856"
---
```powershell

Import-Module Microsoft.Graph.Education

$params = @{
    "@odata.type" = "#microsoft.graph.educationPointsOutcome"
    Points = @{
        "@odata.type" = "#microsoft.graph.educationAssignmentPointsGrade"
        Points = 
    }
}

Update-MgEducationClassAssignmentSubmissionOutcome -EducationClassId $educationClassId -EducationAssignmentId $educationAssignmentId -EducationSubmissionId $educationSubmissionId -EducationOutcomeId $educationOutcomeId -BodyParameter $params

```