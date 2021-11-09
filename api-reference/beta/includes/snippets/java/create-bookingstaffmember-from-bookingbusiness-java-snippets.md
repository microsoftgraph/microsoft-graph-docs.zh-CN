---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b67b53b8218250f37b5f222e7054279c1917a84b
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60736646"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingStaffMember bookingStaffMember = new BookingStaffMember();
bookingStaffMember.colorIndex = 1;
bookingStaffMember.displayName = "Dana Swope";
bookingStaffMember.emailAddress = "danas@contoso.com";
bookingStaffMember.additionalDataManager().put("role@odata.type", new JsonPrimitive("#microsoft.graph.bookingStaffRole"));
bookingStaffMember.role = BookingStaffRole.EXTERNAL_GUEST;
bookingStaffMember.timeZone = "America/Chicago";
bookingStaffMember.useBusinessHours = true;
bookingStaffMember.additionalDataManager().put("workingHours@odata.type", new JsonPrimitive("#Collection(microsoft.graph.bookingWorkHours)"));
LinkedList<BookingWorkHours> workingHoursList = new LinkedList<BookingWorkHours>();
BookingWorkHours workingHours = new BookingWorkHours();
workingHours.additionalDataManager().put("day@odata.type", new JsonPrimitive("#microsoft.graph.dayOfWeek"));
workingHours.day = DayOfWeek.MONDAY;
workingHours.additionalDataManager().put("timeSlots@odata.type", new JsonPrimitive("#Collection(microsoft.graph.bookingWorkTimeSlot)"));
LinkedList<BookingWorkTimeSlot> timeSlotsList = new LinkedList<BookingWorkTimeSlot>();
BookingWorkTimeSlot timeSlots = new BookingWorkTimeSlot();
timeSlots.end = new TimeOfDay(0, 0, 0);
timeSlots.start = new TimeOfDay(0, 0, 0);
timeSlotsList.add(timeSlots);
workingHours.timeSlots = timeSlotsList;
workingHoursList.add(workingHours);
BookingWorkHours workingHours1 = new BookingWorkHours();
workingHours1.additionalDataManager().put("day@odata.type", new JsonPrimitive("#microsoft.graph.dayOfWeek"));
workingHours1.day = DayOfWeek.TUESDAY;
workingHours1.additionalDataManager().put("timeSlots@odata.type", new JsonPrimitive("#Collection(microsoft.graph.bookingWorkTimeSlot)"));
LinkedList<BookingWorkTimeSlot> timeSlotsList1 = new LinkedList<BookingWorkTimeSlot>();
BookingWorkTimeSlot timeSlots1 = new BookingWorkTimeSlot();
timeSlots1.end = new TimeOfDay(0, 0, 0);
timeSlots1.start = new TimeOfDay(0, 0, 0);
timeSlotsList1.add(timeSlots1);
workingHours1.timeSlots = timeSlotsList1;
workingHoursList.add(workingHours1);
BookingWorkHours workingHours2 = new BookingWorkHours();
workingHours2.additionalDataManager().put("day@odata.type", new JsonPrimitive("#microsoft.graph.dayOfWeek"));
workingHours2.day = DayOfWeek.WEDNESDAY;
workingHours2.additionalDataManager().put("timeSlots@odata.type", new JsonPrimitive("#Collection(microsoft.graph.bookingWorkTimeSlot)"));
LinkedList<BookingWorkTimeSlot> timeSlotsList2 = new LinkedList<BookingWorkTimeSlot>();
BookingWorkTimeSlot timeSlots2 = new BookingWorkTimeSlot();
timeSlots2.end = new TimeOfDay(0, 0, 0);
timeSlots2.start = new TimeOfDay(0, 0, 0);
timeSlotsList2.add(timeSlots2);
workingHours2.timeSlots = timeSlotsList2;
workingHoursList.add(workingHours2);
BookingWorkHours workingHours3 = new BookingWorkHours();
workingHours3.additionalDataManager().put("day@odata.type", new JsonPrimitive("#microsoft.graph.dayOfWeek"));
workingHours3.day = DayOfWeek.THURSDAY;
workingHours3.additionalDataManager().put("timeSlots@odata.type", new JsonPrimitive("#Collection(microsoft.graph.bookingWorkTimeSlot)"));
LinkedList<BookingWorkTimeSlot> timeSlotsList3 = new LinkedList<BookingWorkTimeSlot>();
BookingWorkTimeSlot timeSlots3 = new BookingWorkTimeSlot();
timeSlots3.end = new TimeOfDay(0, 0, 0);
timeSlots3.start = new TimeOfDay(0, 0, 0);
timeSlotsList3.add(timeSlots3);
workingHours3.timeSlots = timeSlotsList3;
workingHoursList.add(workingHours3);
BookingWorkHours workingHours4 = new BookingWorkHours();
workingHours4.additionalDataManager().put("day@odata.type", new JsonPrimitive("#microsoft.graph.dayOfWeek"));
workingHours4.day = DayOfWeek.FRIDAY;
workingHours4.additionalDataManager().put("timeSlots@odata.type", new JsonPrimitive("#Collection(microsoft.graph.bookingWorkTimeSlot)"));
LinkedList<BookingWorkTimeSlot> timeSlotsList4 = new LinkedList<BookingWorkTimeSlot>();
BookingWorkTimeSlot timeSlots4 = new BookingWorkTimeSlot();
timeSlots4.end = new TimeOfDay(0, 0, 0);
timeSlots4.start = new TimeOfDay(0, 0, 0);
timeSlotsList4.add(timeSlots4);
workingHours4.timeSlots = timeSlotsList4;
workingHoursList.add(workingHours4);
bookingStaffMember.workingHours = workingHoursList;

graphClient.bookingBusinesses("{id}").staffMembers()
    .buildRequest()
    .post(bookingStaffMember);

```