---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9bf6ce51c26cd77c56f47f5b0b256daa8f1b5afc
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62109509"
---
```powershell

Import-Module Microsoft.Graph.Calendar

Remove-MgUserCalendarGroup -UserId $userId -CalendarGroupId $calendarGroupId

```