---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 914737570e491ed8a3a6be98cdb5ead442c64fe0
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62109138"
---
```powershell

Import-Module Microsoft.Graph.Education

Remove-MgEducationClassAssignmentResource -EducationClassId $educationClassId -EducationAssignmentId $educationAssignmentId -EducationAssignmentResourceId $educationAssignmentResourceId

```