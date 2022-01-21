---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f0d1bbd6ce5c872980d05614aecfbfff3074f9d6
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62099883"
---
```powershell

Import-Module Microsoft.Graph.Education

$params = @{
    Resource = @{
        DisplayName = "_FTP_EDC-61424749-250820211136.pdf"
        FileUrl = "https://graph.microsoft.com/beta/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXodJYOAkI7rTLhw7ME_e42J/items/01QTY63RL45XVPGDBRW5FLDR62Z5TCMGG3"
        "@odata.type" = "#microsoft.graph.educationFileResource"
    }
}

New-MgEducationClassAssignmentSubmissionResource -EducationClassId $educationClassId -EducationAssignmentId $educationAssignmentId -EducationSubmissionId $educationSubmissionId -BodyParameter $params

```