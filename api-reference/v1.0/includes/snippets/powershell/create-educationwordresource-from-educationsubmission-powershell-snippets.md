---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7656cf0df8e9b55c3935530d9ce7ff865f536bfe
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62092319"
---
```powershell

Import-Module Microsoft.Graph.Education

$params = @{
    Resource = @{
        "@odata.type" = "microsoft.graph.educationWordResource"
        DisplayName = "Report.docx"
        FileUrl = "https://graph.microsoft.com/v1.0/drives/b!DPA6q59Tw0mtgmyXRUmrQRqBZTesG-lMkl1cBmvvMeUEWrOk89nKRpUEr4ZhNYBc/items/016XPCQEELISJB7NVNVBAK7V4UIF6Q27U2"
    }
}

New-MgEducationClassAssignmentSubmissionResource -EducationClassId $educationClassId -EducationAssignmentId $educationAssignmentId -EducationSubmissionId $educationSubmissionId -BodyParameter $params

```