---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 38d9ac8880f6c9607a9ab0f8286f328cdf3daf6a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865480"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingStaffMember = new BookingStaffMember
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"workingHours@odata.type","#Collection(microsoft.graph.bookingWorkHours)"},
        {"role@odata.type","#microsoft.graph.bookingStaffRole"},
        {"@odata.type","#microsoft.graph.bookingStaffMember"}
    },
    ColorIndex = 1,
    DisplayName = "Dana Swope",
    EmailAddress = "danas@contoso.com",
    Role = BookingStaffRole.ExternalGuest,
    UseBusinessHours = true,
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

await graphClient.BookingBusinesses["{id}"].StaffMembers
    .Request()
    .AddAsync(bookingStaffMember);

```