---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a0a78036bd6bfb841ad33dde7d482992623425e1
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349776"
---
```powershell

Import-Module Microsoft.Graph.Calendar

# A UPN can also be used as -UserId.
Remove-MgUserCalendarGroup -UserId $userId -CalendarGroupId $calendarGroupId

```