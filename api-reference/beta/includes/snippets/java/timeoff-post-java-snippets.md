---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8f6df1dce9b086b00188022d08808dbcd78f2092
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35870784"
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