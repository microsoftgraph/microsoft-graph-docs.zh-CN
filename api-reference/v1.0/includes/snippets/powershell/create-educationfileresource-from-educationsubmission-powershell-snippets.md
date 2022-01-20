---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1d9449b4259f3b694834d0fb4cee6ddf0c31f89a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62092317"
---
```powershell

Import-Module Microsoft.Graph.Education

$params = @{
    Resource = @{
        DisplayName = "_FTP_EDC-61424749-250820211136.pdf"
        FileUrl = "https://graph.microsoft.com/v1.0/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXodJYOAkI7rTLhw7ME_e42J/items/01QTY63RL45XVPGDBRW5FLDR62Z5TCMGG3"
        "@odata.type" = "#microsoft.graph.educationFileResource"
    }
}

New-MgEducationClassAssignmentSubmissionResource -EducationClassId $educationClassId -EducationAssignmentId $educationAssignmentId -EducationSubmissionId $educationSubmissionId -BodyParameter $params

```