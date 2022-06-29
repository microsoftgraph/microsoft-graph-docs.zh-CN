---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 35dd62dcf2ba307b723ad03b2aaf41eaa7ea50e6
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66445951"
---
```powershell

Import-Module Microsoft.Graph.Education

$params = @{
    "@odata.id" = "https://graph.microsoft.com/v1.0/education/me/rubrics/ceb3863e-6912-4ea9-ac41-3c2bb7b6672d"
}

Set-MgEducationClassAssignmentRubricByRef -EducationClassId $educationClassId -EducationAssignmentId $educationAssignmentId -BodyParameter $params

```