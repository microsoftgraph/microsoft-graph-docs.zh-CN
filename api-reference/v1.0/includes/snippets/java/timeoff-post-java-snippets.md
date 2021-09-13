---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7c94e30bdff51afdebf9d0af5bfd770ea9a2a390d4068041a585660e448e8db4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274435"
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