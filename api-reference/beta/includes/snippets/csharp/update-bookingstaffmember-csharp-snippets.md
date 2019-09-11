---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ef87162521e3af879c680dd92faf278ca74a00ef
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/11/2019
ms.locfileid: "36845928"
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
                {"day@odata.type","#microsoft.graph.dayOfWeek"},
                {"@odata.type","#microsoft.graph.bookingWorkHours"}
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
                {"day@odata.type","#microsoft.graph.dayOfWeek"},
                {"@odata.type","#microsoft.graph.bookingWorkHours"}
            },
            Day = DayOfWeek.Tuesday,
            TimeSlots = new List<BookingWorkTimeSlot>()
            {
                new BookingWorkTimeSlot
                {
                    AdditionalData = new Dictionary<string, object>()
                    {
                        {"@odata.type","#microsoft.graph.bookingWorkTimeSlot"}
                    },
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
                {"day@odata.type","#microsoft.graph.dayOfWeek"},
                {"@odata.type","#microsoft.graph.bookingWorkHours"}
            },
            Day = DayOfWeek.Wednesday,
            TimeSlots = new List<BookingWorkTimeSlot>()
            {
                new BookingWorkTimeSlot
                {
                    AdditionalData = new Dictionary<string, object>()
                    {
                        {"@odata.type","#microsoft.graph.bookingWorkTimeSlot"}
                    },
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
                {"day@odata.type","#microsoft.graph.dayOfWeek"},
                {"@odata.type","#microsoft.graph.bookingWorkHours"}
            },
            Day = DayOfWeek.Thursday,
            TimeSlots = new List<BookingWorkTimeSlot>()
            {
                new BookingWorkTimeSlot
                {
                    AdditionalData = new Dictionary<string, object>()
                    {
                        {"@odata.type","#microsoft.graph.bookingWorkTimeSlot"}
                    },
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
                {"day@odata.type","#microsoft.graph.dayOfWeek"},
                {"@odata.type","#microsoft.graph.bookingWorkHours"}
            },
            Day = DayOfWeek.Friday,
            TimeSlots = new List<BookingWorkTimeSlot>()
            {
                new BookingWorkTimeSlot
                {
                    AdditionalData = new Dictionary<string, object>()
                    {
                        {"@odata.type","#microsoft.graph.bookingWorkTimeSlot"}
                    },
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