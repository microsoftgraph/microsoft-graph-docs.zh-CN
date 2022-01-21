---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8df80f7747e6ccea5d673ace4a55df58894b44aa
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62111360"
---
```powershell

Import-Module Microsoft.Graph.Education

$params = @{
    AddedStudentAction = "assignIfOpen"
    NotificationChannelUrl = "https://graph.microsoft.com/beta/teams('acdefc6b-2dc6-4e71-b1e9-6d9810ab1793')/channels('3da03fc4-8eac-4459-84fb-1422dc01f65e')"
}

Update-MgEducationClassAssignmentDefault -EducationClassId $educationClassId -BodyParameter $params

```