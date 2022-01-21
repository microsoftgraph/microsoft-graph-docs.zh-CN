---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c158366d7ba813a1d73377e6a0fb0e353d503ed0
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62109089"
---
```powershell

Import-Module Microsoft.Graph.Education

$params = @{
    "@odata.id" = "https://graph.microsoft.com/beta/education/users/14011"
}

New-MgEducationClassTeacherByRef -EducationClassId $educationClassId -BodyParameter $params

```