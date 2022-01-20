---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce68ae8eb006418aa549811c32bf076ca8903efc
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62095326"
---
```powershell

Import-Module Microsoft.Graph.Calendar

Get-MgUserCalendarGroup -UserId $userId -CalendarGroupId $calendarGroupId

```