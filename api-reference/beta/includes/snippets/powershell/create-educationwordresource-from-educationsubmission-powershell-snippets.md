---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0f28b2d4b1478539fb27237869b344edea2f5ae6
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62099884"
---
```powershell

Import-Module Microsoft.Graph.Education

$params = @{
    Resource = @{
        "@odata.type" = "microsoft.graph.educationWordResource"
        DisplayName = "Report.docx"
        FileUrl = "https://graph.microsoft.com/beta/drives/b!DPA6q59Tw0mtgmyXRUmrQRqBZTesG-lMkl1cBmvvMeUEWrOk89nKRpUEr4ZhNYBc/items/016XPCQEELISJB7NVNVBAK7V4UIF6Q27U2"
    }
}

New-MgEducationClassAssignmentSubmissionResource -EducationClassId $educationClassId -EducationAssignmentId $educationAssignmentId -EducationSubmissionId $educationSubmissionId -BodyParameter $params

```