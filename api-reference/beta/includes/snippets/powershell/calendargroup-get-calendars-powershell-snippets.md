---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d51f6e24c9d642df8f8c459b314ef84fbaa139ea
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62124052"
---
```powershell

Import-Module Microsoft.Graph.Calendar

Get-MgUserCalendarGroupCalendar -UserId $userId -CalendarGroupId $calendarGroupId

```