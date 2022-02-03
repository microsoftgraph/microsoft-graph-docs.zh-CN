---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6916fa68f4ebb9aa78f4ca11eb16f0257b330840
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62343585"
---
```powershell

Import-Module Microsoft.Graph.Education

Invoke-MgReassignEducationClassAssignmentSubmission -EducationClassId $educationClassId -EducationAssignmentId $educationAssignmentId -EducationSubmissionId $educationSubmissionId

```