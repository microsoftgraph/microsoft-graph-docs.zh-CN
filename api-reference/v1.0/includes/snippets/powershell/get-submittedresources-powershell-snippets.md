---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 12a5685fbbef022d69b6d12e45bf0ec20198ec01
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62114994"
---
```powershell

Import-Module Microsoft.Graph.Education

Get-MgEducationClassAssignmentSubmissionSubmittedResource -EducationClassId $educationClassId -EducationAssignmentId $educationAssignmentId -EducationSubmissionId $educationSubmissionId

```