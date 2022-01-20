---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 67707844d87a3cbce4591803a93171ea0dddbdfb
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62099885"
---
```powershell

Import-Module Microsoft.Graph.Education

$params = @{
    Resource = @{
        "@odata.type" = "#microsoft.graph.educationPowerPointResource"
        DisplayName = "state diagram.pptx"
        FileUrl = "https://graph.microsoft.com/beta/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXodJYOAkI7rTLhw7ME_e42J/items/01QTY63RN3MHWWM7BNXJD2UD5OMRFEDKN2"
    }
}

New-MgEducationClassAssignmentSubmissionResource -EducationClassId $educationClassId -EducationAssignmentId $educationAssignmentId -EducationSubmissionId $educationSubmissionId -BodyParameter $params

```