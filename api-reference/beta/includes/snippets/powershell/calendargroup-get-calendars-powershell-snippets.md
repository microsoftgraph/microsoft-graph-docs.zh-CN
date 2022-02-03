---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 697ca8499d311c184b24c4635a849d7a090a101e
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350156"
---
```powershell

Import-Module Microsoft.Graph.Calendar

# A UPN can also be used as -UserId.
Get-MgUserCalendarGroupCalendar -UserId $userId -CalendarGroupId $calendarGroupId

```