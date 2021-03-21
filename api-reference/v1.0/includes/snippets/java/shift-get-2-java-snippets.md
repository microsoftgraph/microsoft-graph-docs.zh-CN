---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 54362bce5b672031a4d65462421880520a04035b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954746"
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
LinkedList<DayOfWeek> daysOfWeekList = new LinkedList<DayOfWeek>();
daysOfWeekList.add(DayOfWeek.MONDAY);
daysOfWeekList.add(DayOfWeek.WEDNESDAY);
daysOfWeekList.add(DayOfWeek.FRIDAY);
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