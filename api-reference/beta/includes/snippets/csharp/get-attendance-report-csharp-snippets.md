---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3956dd2ea9400d3ed42916518f6aab25d9f4f1b0
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996432"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var meetingAttendanceReport = await graphClient.Me.OnlineMeetings["{onlineMeeting-id}"].MeetingAttendanceReport
    .Request()
    .GetAsync();

```