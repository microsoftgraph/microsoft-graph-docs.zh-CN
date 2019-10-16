---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f624fbb7b4aff7c6dac5971ae25f1cdb719c13d
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37544178"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingStaffMember = new BookingStaffMember
{
    WorkingHours = new List<BookingWorkHours>()
    {
        new BookingWorkHours
        {
            AdditionalData = new Dictionary<string, object>()
            {
                {"timeSlots@odata.type","#Collection(microsoft.graph.bookingWorkTimeSlot)"},
                {"day@odata.type","#microsoft.graph.dayOfWeek"}
            },
            Day = DayOfWeek.Monday,
            TimeSlots = new List<BookingWorkTimeSlot>()
            {
            }
        },
        new BookingWorkHours
        {
            AdditionalData = new Dictionary<string, object>()
            {
                {"timeSlots@odata.type","#Collection(microsoft.graph.bookingWorkTimeSlot)"},
                {"day@odata.type","#microsoft.graph.dayOfWeek"}
            },
            Day = DayOfWeek.Tuesday,
            TimeSlots = new List<BookingWorkTimeSlot>()
            {
                new BookingWorkTimeSlot
                {
                    End = "17:00:00.0000000",
                    Start = "08:00:00.0000000"
                }
            }
        },
        new BookingWorkHours
        {
            AdditionalData = new Dictionary<string, object>()
            {
                {"timeSlots@odata.type","#Collection(microsoft.graph.bookingWorkTimeSlot)"},
                {"day@odata.type","#microsoft.graph.dayOfWeek"}
            },
            Day = DayOfWeek.Wednesday,
            TimeSlots = new List<BookingWorkTimeSlot>()
            {
                new BookingWorkTimeSlot
                {
                    End = "17:00:00.0000000",
                    Start = "08:00:00.0000000"
                }
            }
        },
        new BookingWorkHours
        {
            AdditionalData = new Dictionary<string, object>()
            {
                {"timeSlots@odata.type","#Collection(microsoft.graph.bookingWorkTimeSlot)"},
                {"day@odata.type","#microsoft.graph.dayOfWeek"}
            },
            Day = DayOfWeek.Thursday,
            TimeSlots = new List<BookingWorkTimeSlot>()
            {
                new BookingWorkTimeSlot
                {
                    End = "17:00:00.0000000",
                    Start = "08:00:00.0000000"
                }
            }
        },
        new BookingWorkHours
        {
            AdditionalData = new Dictionary<string, object>()
            {
                {"timeSlots@odata.type","#Collection(microsoft.graph.bookingWorkTimeSlot)"},
                {"day@odata.type","#microsoft.graph.dayOfWeek"}
            },
            Day = DayOfWeek.Friday,
            TimeSlots = new List<BookingWorkTimeSlot>()
            {
                new BookingWorkTimeSlot
                {
                    End = "17:00:00.0000000",
                    Start = "08:00:00.0000000"
                }
            }
        }
    }
};

await graphClient.BookingBusinesses["Contosolunchdelivery@M365B489948.onmicrosoft.com"].StaffMembers["8ee1c803-a1fa-406d-8259-7ab53233f148"]
    .Request()
    .UpdateAsync(bookingStaffMember);

```