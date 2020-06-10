---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 359bc10e6bc211cd1474c6a1c83312f56eb32a35
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44685071"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingStaffMember = new BookingStaffMember
{
    WorkingHours = new List<BookingWorkHours>()
    {
        new BookingWorkHours
        {
            Day = DayOfWeek.Monday,
            TimeSlots = new List<BookingWorkTimeSlot>()
            {
            },
            AdditionalData = new Dictionary<string, object>()
            {
                {"day@odata.type", "#microsoft.graph.dayOfWeek"},
                {"timeSlots@odata.type", "#Collection(microsoft.graph.bookingWorkTimeSlot)"}
            }
        },
        new BookingWorkHours
        {
            Day = DayOfWeek.Tuesday,
            TimeSlots = new List<BookingWorkTimeSlot>()
            {
                new BookingWorkTimeSlot
                {
                    End = new TimeOfDay(17, 0, 0),
                    Start = new TimeOfDay(8, 0, 0)
                }
            },
            AdditionalData = new Dictionary<string, object>()
            {
                {"day@odata.type", "#microsoft.graph.dayOfWeek"},
                {"timeSlots@odata.type", "#Collection(microsoft.graph.bookingWorkTimeSlot)"}
            }
        },
        new BookingWorkHours
        {
            Day = DayOfWeek.Wednesday,
            TimeSlots = new List<BookingWorkTimeSlot>()
            {
                new BookingWorkTimeSlot
                {
                    End = new TimeOfDay(17, 0, 0),
                    Start = new TimeOfDay(8, 0, 0)
                }
            },
            AdditionalData = new Dictionary<string, object>()
            {
                {"day@odata.type", "#microsoft.graph.dayOfWeek"},
                {"timeSlots@odata.type", "#Collection(microsoft.graph.bookingWorkTimeSlot)"}
            }
        },
        new BookingWorkHours
        {
            Day = DayOfWeek.Thursday,
            TimeSlots = new List<BookingWorkTimeSlot>()
            {
                new BookingWorkTimeSlot
                {
                    End = new TimeOfDay(17, 0, 0),
                    Start = new TimeOfDay(8, 0, 0)
                }
            },
            AdditionalData = new Dictionary<string, object>()
            {
                {"day@odata.type", "#microsoft.graph.dayOfWeek"},
                {"timeSlots@odata.type", "#Collection(microsoft.graph.bookingWorkTimeSlot)"}
            }
        },
        new BookingWorkHours
        {
            Day = DayOfWeek.Friday,
            TimeSlots = new List<BookingWorkTimeSlot>()
            {
                new BookingWorkTimeSlot
                {
                    End = new TimeOfDay(17, 0, 0),
                    Start = new TimeOfDay(8, 0, 0)
                }
            },
            AdditionalData = new Dictionary<string, object>()
            {
                {"day@odata.type", "#microsoft.graph.dayOfWeek"},
                {"timeSlots@odata.type", "#Collection(microsoft.graph.bookingWorkTimeSlot)"}
            }
        }
    }
};

await graphClient.BookingBusinesses["Contosolunchdelivery@M365B489948.onmicrosoft.com"].StaffMembers["8ee1c803-a1fa-406d-8259-7ab53233f148"]
    .Request()
    .UpdateAsync(bookingStaffMember);

```