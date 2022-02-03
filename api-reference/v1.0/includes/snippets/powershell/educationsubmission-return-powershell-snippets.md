---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f4516b84269e3d4e2a9c2a1bc10fb0659408b8ca
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62343829"
---
```powershell

Import-Module Microsoft.Graph.Education

Invoke-MgReturnEducationClassAssignmentSubmission -EducationClassId $educationClassId -EducationAssignmentId $educationAssignmentId -EducationSubmissionId $educationSubmissionId

```