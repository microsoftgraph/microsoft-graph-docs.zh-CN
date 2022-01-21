---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ad518134c80d8e2d8993a4d1dd242ef07e26c8de
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62119179"
---
```powershell

Import-Module Microsoft.Graph.Education

$params = @{
    "@odata.id" = "https://graph.microsoft.com/beta/education/users/13015"
}

New-MgEducationClassMemberByRef -EducationClassId $educationClassId -BodyParameter $params

```