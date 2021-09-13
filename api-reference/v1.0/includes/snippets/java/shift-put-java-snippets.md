---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ada1ee40c15d5744362c1fd790888cea1234d014c5e7b13bd06480ea234cb048
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278697"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "return=representation"));

Shift shift = new Shift();
shift.id = "SHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8";
shift.createdDateTime = OffsetDateTimeSerializer.deserialize("2019-03-14T04:32:51.451Z");
shift.lastModifiedDateTime = OffsetDateTimeSerializer.deserialize("2019-03-14T05:32:51.451Z");
shift.userId = "c5d0c76b-80c4-481c-be50-923cd8d680a1";
shift.schedulingGroupId = "TAG_228940ed-ff84-4e25-b129-1b395cf78be0";
IdentitySet lastModifiedBy = new IdentitySet();
lastModifiedBy.application = null;
lastModifiedBy.device = null;
lastModifiedBy.conversation = null;
Identity user = new Identity();
user.id = "366c0b19-49b1-41b5-a03f-9f3887bd0ed8";
user.displayName = "John Doe";
lastModifiedBy.user = user;
shift.lastModifiedBy = lastModifiedBy;
ShiftItem sharedShift = new ShiftItem();
sharedShift.displayName = "Day shift";
sharedShift.notes = "Please do inventory as part of your shift.";
sharedShift.startDateTime = OffsetDateTimeSerializer.deserialize("2019-03-11T15:00:00Z");
sharedShift.endDateTime = OffsetDateTimeSerializer.deserialize("2019-03-12T00:00:00Z");
sharedShift.theme = ScheduleEntityTheme.BLUE;
LinkedList<ShiftActivity> activitiesList = new LinkedList<ShiftActivity>();
ShiftActivity activities = new ShiftActivity();
activities.isPaid = true;
activities.startDateTime = OffsetDateTimeSerializer.deserialize("2019-03-11T15:00:00Z");
activities.endDateTime = OffsetDateTimeSerializer.deserialize("2019-03-11T15:15:00Z");
activities.code = "";
activities.displayName = "Lunch";
activitiesList.add(activities);
sharedShift.activities = activitiesList;
shift.sharedShift = sharedShift;
ShiftItem draftShift = new ShiftItem();
draftShift.displayName = "Day shift";
draftShift.notes = "Please do inventory as part of your shift.";
draftShift.startDateTime = OffsetDateTimeSerializer.deserialize("2019-03-11T15:00:00Z");
draftShift.endDateTime = OffsetDateTimeSerializer.deserialize("2019-03-12T00:00:00Z");
draftShift.theme = ScheduleEntityTheme.BLUE;
LinkedList<ShiftActivity> activitiesList1 = new LinkedList<ShiftActivity>();
ShiftActivity activities1 = new ShiftActivity();
activities1.isPaid = true;
activities1.startDateTime = OffsetDateTimeSerializer.deserialize("2019-03-11T15:00:00Z");
activities1.endDateTime = OffsetDateTimeSerializer.deserialize("2019-03-11T15:30:00Z");
activities1.code = "";
activities1.displayName = "Lunch";
activitiesList1.add(activities1);
draftShift.activities = activitiesList1;
shift.draftShift = draftShift;

graphClient.teams("{teamId}").schedule().shifts("{shiftId}")
    .buildRequest( requestOptions )
    .patch(shift);

```