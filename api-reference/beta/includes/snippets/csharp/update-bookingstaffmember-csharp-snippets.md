---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1c86de2052a5878f2d14e9f2d23a7f1aea76cdd9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865199"
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
            TimeSlots = new List<String>()
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