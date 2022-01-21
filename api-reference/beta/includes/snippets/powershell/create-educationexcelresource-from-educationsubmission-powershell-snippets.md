---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 12a0713d03bd3abe328f9a7ab3caa9e7ac13bde5
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62099882"
---
```powershell

Import-Module Microsoft.Graph.Education

$params = @{
    Resource = @{
        "@odata.type" = "#microsoft.graph.educationExcelResource"
        DisplayName = "userAgeGroup QueryParameter Test.xlsx"
        FileUrl = "https://graph.microsoft.com/beta/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXodJYOAkI7rTLhw7ME_e42J/items/01QTY63RONPUDM2CZKNRF3TGHYUM7Z64WE"
    }
}

New-MgEducationClassAssignmentSubmissionResource -EducationClassId $educationClassId -EducationAssignmentId $educationAssignmentId -EducationSubmissionId $educationSubmissionId -BodyParameter $params

```