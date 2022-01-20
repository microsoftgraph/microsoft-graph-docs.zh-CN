---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6f2dc1f33996f061ae6609479b65e58cb76b4ca2
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62124016"
---
```powershell

Import-Module Microsoft.Graph.Calendar

$params = @{
    Name = "Marketing calendar"
}

New-MgUserCalendarGroupCalendar -UserId $userId -CalendarGroupId $calendarGroupId -BodyParameter $params

```