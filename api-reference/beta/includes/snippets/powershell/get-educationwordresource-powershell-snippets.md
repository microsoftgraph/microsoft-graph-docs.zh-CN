---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f694324f12a573b20dc5e1b6b981741022d93c08
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62120657"
---
```powershell

Import-Module Microsoft.Graph.Education

Get-MgEducationClassAssignmentSubmissionResource -EducationClassId $educationClassId -EducationAssignmentId $educationAssignmentId -EducationSubmissionId $educationSubmissionId -EducationSubmissionResourceId $educationSubmissionResourceId

```