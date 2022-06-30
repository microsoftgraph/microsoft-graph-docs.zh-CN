---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 56c7946e78491a755b3ebf7a45b4ae845c263b5e
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447030"
---
```powershell

Import-Module Microsoft.Graph.Education

Remove-MgEducationClassAssignmentRubricByRef -EducationClassId $educationClassId -EducationAssignmentId $educationAssignmentId

```