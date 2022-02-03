---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1cf0c9ea8bbca520fd93d4ab588a9e6734b1a9ba
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351727"
---
```powershell

Import-Module Microsoft.Graph.Calendar

$params = @{
    Name = "Marketing calendar"
}

# A UPN can also be used as -UserId.
New-MgUserCalendarGroupCalendar -UserId $userId -CalendarGroupId $calendarGroupId -BodyParameter $params

```