---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d3f6f6dc9a9671e2ec6dad5c777e1602c1b334f7
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62097811"
---
```powershell

Import-Module Microsoft.Graph.Education

$params = @{
    "@odata.id" = "https://graph.microsoft.com/v1.0/education/users/14011"
}

New-MgEducationClassTeacherByRef -EducationClassId $educationClassId -BodyParameter $params

```