---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: efc4d164996b3bf91cd1b374308ac7fa6ca82e92
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62103208"
---
```powershell

Import-Module Microsoft.Graph.Education

$params = @{
    DistributeForStudentWork = $false
    Resource = @{
        "@odata.type" = "microsoft.graph.educationPowerPointResource"
        DisplayName = "state diagram.pptx"
        FileUrl = "https://graph.microsoft.com/beta/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXoOOmEQNO79QpIMPdOmY3nf/items/01QTY63RN327OXRN6EVFE2Q5FRJZTN5EOJ"
    }
}

New-MgEducationClassAssignmentResource -EducationClassId $educationClassId -EducationAssignmentId $educationAssignmentId -BodyParameter $params

```