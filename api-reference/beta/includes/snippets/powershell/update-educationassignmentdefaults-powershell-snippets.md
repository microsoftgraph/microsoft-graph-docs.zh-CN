---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d316873d0b87701676eca1403c64fbc730e96e3c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62113811"
---
```powershell

Import-Module Microsoft.Graph.Education

$params = @{
    AddedStudentAction = "assignIfOpen"
    AddToCalendarAction = "studentsAndTeamOwners"
    NotificationChannelUrl = "https://graph.microsoft.com/beta/teams('id')/channels('id')"
}

Update-MgEducationClassAssignmentDefault -EducationClassId $educationClassId -BodyParameter $params

```