---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f0e169a8d609e5135e577e70f00855d99bc8df2d
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37544177"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingStaffMember = new BookingStaffMember
{
    ColorIndex = 1,
    DisplayName = "Dana Swope",
    EmailAddress = "danas@contoso.com",
    AdditionalData = new Dictionary<string, object>()
    {
        {"workingHours@odata.type","#Collection(microsoft.graph.bookingWorkHours)"},
        {"role@odata.type","#microsoft.graph.bookingStaffRole"}
    },
    Role = BookingStaffRole.ExternalGuest,
    UseBusinessHours = true,
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

await graphClient.BookingBusinesses["{id}"].StaffMembers
    .Request()
    .AddAsync(bookingStaffMember);

```