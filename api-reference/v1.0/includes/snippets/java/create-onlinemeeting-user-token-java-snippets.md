---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a78fabf3e4cf85b8b07cca70b39ce6d5210464f1
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865861"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OnlineMeeting onlineMeeting = new OnlineMeeting();
onlineMeeting.startDateTime = "2019-07-12T21:30:34.2444915+00:00";
onlineMeeting.endDateTime = "2019-07-12T22:00:34.2464912+00:00";
onlineMeeting.subject = "User Token Meeting";

graphClient.me().onlineMeetings()
    .buildRequest()
    .post(onlineMeeting);

```