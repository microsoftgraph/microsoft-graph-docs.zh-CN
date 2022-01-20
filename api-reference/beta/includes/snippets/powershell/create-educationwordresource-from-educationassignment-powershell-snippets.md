---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1d1502dd7d92079e75419766d25984eef1645fc8
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62103206"
---
```powershell

Import-Module Microsoft.Graph.Education

$params = @{
    DistributeForStudentWork = $false
    Resource = @{
        "@odata.type" = "microsoft.graph.educationWordResource"
        DisplayName = "Issues and PR in guthub.docx"
        FileUrl = "https://graph.microsoft.com/beta/drives/b!DPA6q59Tw0mtgmyXRUmrQRqBZTesG-lMkl1cBmvvMeUEWrOk89nKRpUEr4ZhNYBc/items/016XPCQEELISJB7NVNVBAK7V4UIF6Q27U2"
    }
}

New-MgEducationClassAssignmentResource -EducationClassId $educationClassId -EducationAssignmentId $educationAssignmentId -BodyParameter $params

```