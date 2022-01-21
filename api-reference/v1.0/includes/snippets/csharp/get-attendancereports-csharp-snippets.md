---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ec0abf1f49b6811f983dda5f078c82fe07eb63d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62104683"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attendanceReports = await graphClient.Me.OnlineMeetings["{onlineMeeting-id}"].AttendanceReports
    .Request()
    .GetAsync();

```