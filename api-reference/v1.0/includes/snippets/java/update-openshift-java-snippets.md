---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e97938b92e0bb3dcdbce54f4c609b55fc68a6341ff5ea2cb48bec61b1f264cc7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218727"
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
    .patch(openShift);

```