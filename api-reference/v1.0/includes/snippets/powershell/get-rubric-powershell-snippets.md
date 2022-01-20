---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a669bb95d6d0456b3c3b09cf9cd5aa5926dab083
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62101151"
---
```powershell

Import-Module Microsoft.Graph.Education

Get-MgEducationClassAssignmentRubric -EducationClassId $educationClassId -EducationAssignmentId $educationAssignmentId

```