---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dd2a7a093610eccd103467c7f3c3ac7014f288b2f738140d20b91496cebd07bf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902409"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var meetingAttendanceReport = await graphClient.Me.OnlineMeetings["{onlineMeeting-id}"].MeetingAttendanceReport
    .Request()
    .GetAsync();

```