---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 71111657f67fb4044ecfb936975cdbef9f46275b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969163"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OnlineMeeting onlineMeeting = new OnlineMeeting();
onlineMeeting.startDateTime = OffsetDateTimeSerializer.deserialize("2020-09-09T21:33:30.8546353+00:00");
onlineMeeting.endDateTime = OffsetDateTimeSerializer.deserialize("2020-09-09T22:03:30.8566356+00:00");
onlineMeeting.subject = "Patch Meeting Subject";

graphClient.me().onlineMeetings("MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi")
    .buildRequest()
    .patch(onlineMeeting);

```