---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf0be236d0b70e486d1d4a607d2a417e5fcd3d4e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62104889"
---
```powershell

Import-Module Microsoft.Graph.Education

$params = @{
    "@odata.id" = "https://graph.microsoft.com/v1.0/education/users/13015"
}

New-MgEducationClassMemberByRef -EducationClassId $educationClassId -BodyParameter $params

```