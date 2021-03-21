---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dfbc9fb409a0239d720a1dca75db06cdd3dd7932
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977795"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OpenShift openShift = new OpenShift();
openShift.schedulingGroupId = "TAG_228940ed-ff84-4e25-b129-1b395cf78be0";
OpenShiftItem sharedOpenShift = new OpenShiftItem();
sharedOpenShift.notes = "Inventory Management";
sharedOpenShift.openSlotCount = 5;
sharedOpenShift.displayName = "Field shift";
sharedOpenShift.startDateTime = OffsetDateTimeSerializer.deserialize("2018-10-04T00:58:45.34Z");
sharedOpenShift.endDateTime = OffsetDateTimeSerializer.deserialize("2018-10-04T09:50:45.332Z");
sharedOpenShift.theme = ScheduleEntityTheme.WHITE;
LinkedList<ShiftActivity> activitiesList = new LinkedList<ShiftActivity>();
ShiftActivity activities = new ShiftActivity();
activities.isPaid = true;
activities.startDateTime = OffsetDateTimeSerializer.deserialize("2018-10-04T00:58:45.34Z");
activities.endDateTime = OffsetDateTimeSerializer.deserialize("2018-10-04T01:58:45.34Z");
activities.code = "";
activities.displayName = "Lunch";
activitiesList.add(activities);
sharedOpenShift.activities = activitiesList;
openShift.sharedOpenShift = sharedOpenShift;
openShift.draftOpenShift = null;

graphClient.teams("{id}").schedule().openShifts("OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8")
    .buildRequest()
    .put(openShift);

```