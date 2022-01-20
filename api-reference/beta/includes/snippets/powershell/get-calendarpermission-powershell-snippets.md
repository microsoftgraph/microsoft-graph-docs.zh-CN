---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 258e055daf6e860743c544fc3cbe57396cdbdfec
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62094473"
---
```powershell

Import-Module Microsoft.Graph.Calendar

Get-MgUserCalendarPermission -UserId $userId -CalendarPermissionId $calendarPermissionId

```