---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8f6df1dce9b086b00188022d08808dbcd78f2092
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44217527"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TimeOff timeOff = new TimeOff();
timeOff.userId = "c5d0c76b-80c4-481c-be50-923cd8d680a1";
TimeOffItem sharedTimeOff = new TimeOffItem();
sharedTimeOff.timeOffReasonId = "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7";
sharedTimeOff.startDateTime = "2019-03-11T07:00:00Z";
sharedTimeOff.endDateTime = "2019-03-12T07:00:00Z";
sharedTimeOff.theme = ScheduleEntityTheme.WHITE;
timeOff.sharedTimeOff = sharedTimeOff;
TimeOffItem draftTimeOff = new TimeOffItem();
draftTimeOff.timeOffReasonId = "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7";
draftTimeOff.startDateTime = "2019-03-11T07:00:00Z";
draftTimeOff.endDateTime = "2019-03-12T07:00:00Z";
draftTimeOff.theme = ScheduleEntityTheme.PINK;
timeOff.draftTimeOff = draftTimeOff;

graphClient.teams("{teamId}").schedule().timesOff()
    .buildRequest()
    .post(timeOff);

```