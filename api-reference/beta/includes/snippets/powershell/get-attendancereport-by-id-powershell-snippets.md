---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5508495ac9c38f903cb2c543680a44a64a0a0bd0
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62130996"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

Get-MgUserOnlineMeetingAttendanceReport -UserId $userId -OnlineMeetingId $onlineMeetingId -MeetingAttendanceReportId $meetingAttendanceReportId -ExpandProperty "attendanceRecords" 

```