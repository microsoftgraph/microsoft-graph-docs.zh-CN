---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 005d2e59a4328723a814626576fa78d64ff8380f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62103088"
---
```powershell

Import-Module Microsoft.Graph.Calendar

Get-MgUserEvent -UserId $userId -EventId $eventId -Property "subject,start,end,occurrenceId,exceptionOccurrences,cancelledOccurrences`$expand" 

```