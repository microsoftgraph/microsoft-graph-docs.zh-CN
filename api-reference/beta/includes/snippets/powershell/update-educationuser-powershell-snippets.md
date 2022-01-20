---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1587cedae56b34a0d74c0514241d0c6b17fdfbf0
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62135121"
---
```powershell

Import-Module Microsoft.Graph.Education

$params = @{
    DisplayName = "Rogelio Cazares"
    GivenName = "Rogelio"
    MiddleName = "Fernando"
    Surname = "Cazares"
}

Update-MgEducationUser -EducationUserId $educationUserId -BodyParameter $params

```