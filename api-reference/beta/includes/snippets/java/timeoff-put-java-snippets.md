---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8fbf3da40b705c84c56627c609454e04bb402b89
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981425"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "return=representation"));

TimeOff timeOff = new TimeOff();
timeOff.userId = "c5d0c76b-80c4-481c-be50-923cd8d680a1";
TimeOffItem sharedTimeOff = new TimeOffItem();
sharedTimeOff.timeOffReasonId = "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7";
sharedTimeOff.startDateTime = CalendarSerializer.deserialize("2019-03-11T07:00:00Z");
sharedTimeOff.endDateTime = CalendarSerializer.deserialize("2019-03-12T07:00:00Z");
sharedTimeOff.theme = ScheduleEntityTheme.WHITE;
timeOff.sharedTimeOff = sharedTimeOff;
TimeOffItem draftTimeOff = new TimeOffItem();
draftTimeOff.timeOffReasonId = "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7";
draftTimeOff.startDateTime = CalendarSerializer.deserialize("2019-03-11T07:00:00Z");
draftTimeOff.endDateTime = CalendarSerializer.deserialize("2019-03-12T07:00:00Z");
draftTimeOff.theme = ScheduleEntityTheme.PINK;
timeOff.draftTimeOff = draftTimeOff;

graphClient.teams("{teamId}").schedule().timesOff("{timeOffId}")
    .buildRequest( requestOptions )
    .put(timeOff);

```