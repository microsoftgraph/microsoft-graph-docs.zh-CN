---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7fd036b6ca8c408d51d4487675faf1449d8c3f05
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61223595"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attendanceRecords = await graphClient.Me.OnlineMeetings["{onlineMeeting-id}"].AttendanceReports["{meetingAttendanceReport-id}"].AttendanceRecords
    .Request()
    .GetAsync();

```