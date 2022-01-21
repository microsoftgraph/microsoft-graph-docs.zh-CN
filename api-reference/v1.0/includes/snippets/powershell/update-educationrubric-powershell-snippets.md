---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cae550793fe510213087e69ea47a4a38e8b927e5
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62092267"
---
```powershell

Import-Module Microsoft.Graph.Education

$params = @{
    DisplayName = "Example Credit Rubric after display name patch"
}

Update-MgEducationMeRubric -EducationRubricId $educationRubricId -BodyParameter $params

```