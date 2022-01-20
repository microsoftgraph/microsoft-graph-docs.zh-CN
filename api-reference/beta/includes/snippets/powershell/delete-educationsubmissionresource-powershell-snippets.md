---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f1573e39aaf1861d509bc5a3e4c322133100d57a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62094129"
---
```powershell

Import-Module Microsoft.Graph.Education

Remove-MgEducationClassAssignmentSubmissionResource -EducationClassId $educationClassId -EducationAssignmentId $educationAssignmentId -EducationSubmissionId $educationSubmissionId -EducationSubmissionResourceId $educationSubmissionResourceId

```