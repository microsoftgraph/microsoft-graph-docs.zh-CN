---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 21681f7ba9cd1a2d0ae2ff0781fa3f7613f39e22
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62346989"
---
```powershell

Import-Module Microsoft.Graph.Education

Invoke-MgUnsubmitEducationClassAssignmentSubmission -EducationClassId $educationClassId -EducationAssignmentId $educationAssignmentId -EducationSubmissionId $educationSubmissionId

```