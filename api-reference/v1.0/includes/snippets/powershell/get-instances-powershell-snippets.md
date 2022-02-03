---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a1f80ec0afc5ee32079dd63cf7b1190565d847d9
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350357"
---
```powershell

Import-Module Microsoft.Graph.Calendar

# A UPN can also be used as -UserId.
Get-MgUserEventInstance -UserId $userId -EventId $eventId -Startdatetime "2019-04-08T09:00:00.0000000" -Enddatetime "2019-04-30T09:00:00.0000000" -Property "subject,bodyPreview,seriesMasterId,type,recurrence,start,end" 

```