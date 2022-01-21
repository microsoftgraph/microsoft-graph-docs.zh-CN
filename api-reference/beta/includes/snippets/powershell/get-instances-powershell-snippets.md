---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a7dcda0ed15dbe61c3c3a330aadf24ab252350e2
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62103055"
---
```powershell

Import-Module Microsoft.Graph.Calendar

Get-MgUserEventInstance -UserId $userId -EventId $eventId -Startdatetime "2019-04-08T09:00:00.0000000" -Enddatetime "2019-04-30T09:00:00.0000000" -Property "subject,bodyPreview,seriesMasterId,type,recurrence,start,end" 

```