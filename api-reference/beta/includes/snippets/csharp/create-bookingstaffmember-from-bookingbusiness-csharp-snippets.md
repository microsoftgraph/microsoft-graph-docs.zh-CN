---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c06632d87406b9f8a73fc54be2bdf973799f827
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66502887"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingStaffMember = new BookingStaffMember
{
    ColorIndex = 1,
    DisplayName = "Dana Swope",
    EmailAddress = "danas@contoso.com",
    Role = BookingStaffRole.ExternalGuest,
    TimeZone = "America/Chicago",
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
    IsEmailNotificationEnabled = false,
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