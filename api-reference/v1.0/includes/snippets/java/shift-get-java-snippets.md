---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 012aa568a445215e2f704c1b39ba6f65fc428d07
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684357"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ShiftPreferences shiftPreferences = new ShiftPreferences();
shiftPreferences.id = "SHPR_eeab4fb1-20e5-48ca-ad9b-98119d94bee7";
shiftPreferences.additionalDataManager().put("@odata.etag", new JsonPrimitive("1a371e53-f0a6-4327-a1ee-e3c56e4b38aa"));
LinkedList<ShiftAvailability> availabilityList = new LinkedList<ShiftAvailability>();
ShiftAvailability availability = new ShiftAvailability();
PatternedRecurrence recurrence = new PatternedRecurrence();
RecurrencePattern pattern = new RecurrencePattern();
pattern.type = RecurrencePatternType.WEEKLY;
LinkedList<String> daysOfWeekList = new LinkedList<String>();
daysOfWeekList.add("Monday");
daysOfWeekList.add("Wednesday");
daysOfWeekList.add("Friday");
pattern.daysOfWeek = daysOfWeekList;
pattern.interval = 1;
recurrence.pattern = pattern;
RecurrenceRange range = new RecurrenceRange();
range.type = RecurrenceRangeType.NO_END;
recurrence.range = range;
availability.recurrence = recurrence;
availability.timeZone = "Pacific Standard Time";
availability.timeSlots = null;
availabilityList.add(availability);
shiftPreferences.availability = availabilityList;

graphClient.users("871dbd5c-3a6a-4392-bfe1-042452793a50").settings().shiftPreferences()
    .buildRequest()
    .patch(shiftPreferences);

```