---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa22df4ea44a4ec506f8911efd75b226d79151cb9e43e3261593619511af5d82
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105041"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingStaffMember = new BookingStaffMember
{
    ColorIndex = 1,
    DisplayName = "Dana Swope",
    EmailAddress = "danas@contoso.com",
    Role = BookingStaffRole.ExternalGuest,
    UseBusinessHours = true,
    WorkingHours = new List<BookingWorkHours>()
    {
        new BookingWorkHours
        {
            Day = DayOfWeek.Monday,
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
    },
    AdditionalData = new Dictionary<string, object>()
    {
        {"role@odata.type", "#microsoft.graph.bookingStaffRole"},
        {"workingHours@odata.type", "#Collection(microsoft.graph.bookingWorkHours)"}
    }
};

await graphClient.BookingBusinesses["{bookingBusiness-id}"].StaffMembers
    .Request()
    .AddAsync(bookingStaffMember);

```