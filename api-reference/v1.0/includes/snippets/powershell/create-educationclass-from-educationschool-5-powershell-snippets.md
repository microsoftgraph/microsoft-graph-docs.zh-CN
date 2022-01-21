---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 152e23c9a605ed8ce36d06860c549ac0393c0d68
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62115021"
---
```powershell

Import-Module Microsoft.Graph.Education

$params = @{
    "@odata.id" = "https://graph.microsoft.com/v1.0/education/classes/11006"
}

New-MgEducationSchoolClassByRef -EducationSchoolId $educationSchoolId -BodyParameter $params

```