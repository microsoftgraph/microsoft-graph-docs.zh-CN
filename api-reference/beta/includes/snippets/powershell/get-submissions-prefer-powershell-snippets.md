---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 708fbc5efdb77a8c3727a9a90d593d178244f58c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62103177"
---
```powershell

Import-Module Microsoft.Graph.Education

Get-MgEducationClassAssignmentSubmission -EducationClassId $educationClassId -EducationAssignmentId $educationAssignmentId

```