---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 95f10046e8c74ae42ec51d221e78a9d0cb7113cc
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62099928"
---
```powershell

Import-Module Microsoft.Graph.Education

Get-MgEducationClassAssignmentSubmissionOutcome -EducationClassId $educationClassId -EducationAssignmentId $educationAssignmentId -EducationSubmissionId $educationSubmissionId

```