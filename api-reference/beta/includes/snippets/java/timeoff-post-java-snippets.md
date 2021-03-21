---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cbaf671ecf63d80024ae21d76f315ab4bf3fa55f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969972"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TimeOff timeOff = new TimeOff();
timeOff.userId = "c5d0c76b-80c4-481c-be50-923cd8d680a1";
TimeOffItem sharedTimeOff = new TimeOffItem();
sharedTimeOff.timeOffReasonId = "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7";
sharedTimeOff.startDateTime = OffsetDateTimeSerializer.deserialize("2019-03-11T07:00:00Z");
sharedTimeOff.endDateTime = OffsetDateTimeSerializer.deserialize("2019-03-12T07:00:00Z");
sharedTimeOff.theme = ScheduleEntityTheme.WHITE;
timeOff.sharedTimeOff = sharedTimeOff;
TimeOffItem draftTimeOff = new TimeOffItem();
draftTimeOff.timeOffReasonId = "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7";
draftTimeOff.startDateTime = OffsetDateTimeSerializer.deserialize("2019-03-11T07:00:00Z");
draftTimeOff.endDateTime = OffsetDateTimeSerializer.deserialize("2019-03-12T07:00:00Z");
draftTimeOff.theme = ScheduleEntityTheme.PINK;
timeOff.draftTimeOff = draftTimeOff;

graphClient.teams("{teamId}").schedule().timesOff()
    .buildRequest()
    .post(timeOff);

```