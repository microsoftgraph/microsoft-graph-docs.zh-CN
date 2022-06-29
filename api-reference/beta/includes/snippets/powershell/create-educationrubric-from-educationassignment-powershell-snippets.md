---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 44ec137adf2c31619226631dd3ca53e2e9736aa1
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66436328"
---
```powershell

Import-Module Microsoft.Graph.Education

$params = @{
    "@odata.id" = "https://graph.microsoft.com/v1.0/education/me/rubrics/{id}"
}

Set-MgEducationClassAssignmentRubricByRef -EducationClassId $educationClassId -EducationAssignmentId $educationAssignmentId -BodyParameter $params

```