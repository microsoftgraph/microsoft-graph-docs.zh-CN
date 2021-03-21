---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 77120bfb33fac75d8a487d23f0cd201d2d8680d4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975180"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OnlineMeeting onlineMeeting = new OnlineMeeting();
onlineMeeting.startDateTime = OffsetDateTimeSerializer.deserialize("2019-07-12T21:30:34.2444915+00:00");
onlineMeeting.endDateTime = OffsetDateTimeSerializer.deserialize("2019-07-12T22:00:34.2464912+00:00");
onlineMeeting.subject = "User Token Meeting";

graphClient.me().onlineMeetings()
    .buildRequest()
    .post(onlineMeeting);

```