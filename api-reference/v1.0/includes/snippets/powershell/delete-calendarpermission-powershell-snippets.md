---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a4c7358f7f76ef2fcfc5e4eba310f6c793ec1f96
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62115106"
---
```powershell

Import-Module Microsoft.Graph.Calendar

Remove-MgUserCalendarPermission -UserId $userId -CalendarPermissionId $calendarPermissionId

```