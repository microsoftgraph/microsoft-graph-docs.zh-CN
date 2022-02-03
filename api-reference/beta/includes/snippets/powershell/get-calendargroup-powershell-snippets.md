---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bafedf8271bce537a84b4793e7b43d5f8aa29e6d
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352527"
---
```powershell

Import-Module Microsoft.Graph.Calendar

# A UPN can also be used as -UserId.
Get-MgUserCalendarGroup -UserId $userId -CalendarGroupId $calendarGroupId

```