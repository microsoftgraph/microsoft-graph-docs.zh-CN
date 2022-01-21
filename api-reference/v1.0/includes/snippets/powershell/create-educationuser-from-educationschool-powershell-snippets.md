---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 959b0d6209767e23012a6d89cc5fc93f4b4341f1
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62115007"
---
```powershell

Import-Module Microsoft.Graph.Education

$params = @{
    "@odata.id" = "https://graph.microsoft.com/v1.0/education/users/14008"
}

New-MgEducationSchoolUserByRef -EducationSchoolId $educationSchoolId -BodyParameter $params

```