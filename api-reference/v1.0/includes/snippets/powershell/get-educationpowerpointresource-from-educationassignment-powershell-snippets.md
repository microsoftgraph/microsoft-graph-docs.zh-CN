---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 62e7328c4a97c4ef5ef42822c02b5cbbd02af409
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62092401"
---
```powershell

Import-Module Microsoft.Graph.Education

Get-MgEducationClassAssignmentResource -EducationClassId $educationClassId -EducationAssignmentId $educationAssignmentId -EducationAssignmentResourceId $educationAssignmentResourceId

```