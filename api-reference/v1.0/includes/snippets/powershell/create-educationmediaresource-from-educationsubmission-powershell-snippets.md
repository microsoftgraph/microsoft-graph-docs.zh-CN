---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ea517dddf1a7eb6d9972af35c56087d17c31409
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62092315"
---
```powershell

Import-Module Microsoft.Graph.Education

$params = @{
    Resource = @{
        DisplayName = "category.jpg"
        FileUrl = "https://graph.microsoft.com/v1.0/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXodJYOAkI7rTLhw7ME_e42J/items/01QTY63RK2WLKUUBAA4ZBKXNBL6QFC2TKG"
        "@odata.type" = "#microsoft.graph.educationMediaResource"
    }
}

New-MgEducationClassAssignmentSubmissionResource -EducationClassId $educationClassId -EducationAssignmentId $educationAssignmentId -EducationSubmissionId $educationSubmissionId -BodyParameter $params

```