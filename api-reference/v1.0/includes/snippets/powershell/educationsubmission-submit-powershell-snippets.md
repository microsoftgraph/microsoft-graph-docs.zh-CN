---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3701f94c4ceaadb80f1a8eee33b14ca348aa37d
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62340895"
---
```powershell

Import-Module Microsoft.Graph.Education

Submit-MgEducationClassAssignmentSubmission -EducationClassId $educationClassId -EducationAssignmentId $educationAssignmentId -EducationSubmissionId $educationSubmissionId

```