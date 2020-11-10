---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 009c0531e007a15b80fda4a8867e83ac4d47d388
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980103"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OnlineMeeting onlineMeeting = new OnlineMeeting();
onlineMeeting.startDateTime = CalendarSerializer.deserialize("2020-09-09T21:33:30.8546353+00:00");
onlineMeeting.endDateTime = CalendarSerializer.deserialize("2020-09-09T22:03:30.8566356+00:00");
onlineMeeting.subject = "Patch Meeting Subject";

graphClient.me().onlineMeetings("{id}")
    .buildRequest()
    .patch(onlineMeeting);

```