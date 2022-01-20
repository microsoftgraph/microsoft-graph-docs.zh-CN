---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ee8a066ff9e3578adf513a18b8b996fb55f6b25
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62090159"
---
```powershell

Import-Module Microsoft.Graph.Education

$params = @{
    "@odata.id" = "https://graph.microsoft.com/beta/education/classes/11006"
}

New-MgEducationSchoolClassByRef -EducationSchoolId $educationSchoolId -BodyParameter $params

```