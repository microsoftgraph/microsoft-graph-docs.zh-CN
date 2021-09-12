---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eedea303b8b5208d488ef670747b43fa9205aa39ab9831043847eaeaea40a8ff
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221029"
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