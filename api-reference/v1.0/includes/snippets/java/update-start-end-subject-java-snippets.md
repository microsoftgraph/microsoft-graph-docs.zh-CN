---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d9a1978a7068f4fd21db706ad4b0b532d98d3109
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773506"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OnlineMeeting onlineMeeting = new OnlineMeeting();
onlineMeeting.startDateTime = CalendarSerializer.deserialize("2020-09-09T21:33:30.8546353+00:00");
onlineMeeting.endDateTime = CalendarSerializer.deserialize("2020-09-09T22:03:30.8566356+00:00");
onlineMeeting.subject = "Patch Meeting Subject";

graphClient.me().onlineMeetings("MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi")
    .buildRequest()
    .patch(onlineMeeting);

```