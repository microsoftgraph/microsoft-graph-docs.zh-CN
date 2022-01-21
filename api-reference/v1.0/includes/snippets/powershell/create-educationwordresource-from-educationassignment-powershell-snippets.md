---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f4b27daba16b88ff25e9e5f4c191b5e7ba461260
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62128815"
---
```powershell

Import-Module Microsoft.Graph.Education

$params = @{
    DistributeForStudentWork = $false
    Resource = @{
        "@odata.type" = "microsoft.graph.educationWordResource"
        DisplayName = "Issues and PR in guthub.docx"
        FileUrl = "https://graph.microsoft.com/v1.0/drives/b!DPA6q59Tw0mtgmyXRUmrQRqBZTesG-lMkl1cBmvvMeUEWrOk89nKRpUEr4ZhNYBc/items/016XPCQEELISJB7NVNVBAK7V4UIF6Q27U2"
    }
}

New-MgEducationClassAssignmentResource -EducationClassId $educationClassId -EducationAssignmentId $educationAssignmentId -BodyParameter $params

```