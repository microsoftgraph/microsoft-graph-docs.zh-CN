---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3865b56b212cb9ce484c31b1eceb32eae61862df
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66502361"
---
```powershell

Import-Module Microsoft.Graph.Bookings

$params = @{
    "@odata.type" = "#microsoft.graph.bookingStaffMember"
    ColorIndex = 1
    DisplayName = "Dana Swope"
    EmailAddress = "danas@contoso.com"
    "Role@odata.type" = "#microsoft.graph.bookingStaffRole"
    Role = "externalGuest"
    TimeZone = "America/Chicago"
    UseBusinessHours = $true
    "WorkingHours@odata.type" = "#Collection(microsoft.graph.bookingWorkHours)"
    WorkingHours = @(
        @{
            "@odata.type" = "#microsoft.graph.bookingWorkHours"
            "Day@odata.type" = "#microsoft.graph.dayOfWeek"
            Day = "monday"
            "TimeSlots@odata.type" = "#Collection(microsoft.graph.bookingWorkTimeSlot)"
            TimeSlots = @(
                @{
                    "@odata.type" = "#microsoft.graph.bookingWorkTimeSlot"
                    End = "17:00:00.0000000"
                    Start = "08:00:00.0000000"
                }
            )
        }
        @{
            "@odata.type" = "#microsoft.graph.bookingWorkHours"
            "Day@odata.type" = "#microsoft.graph.dayOfWeek"
            Day = "tuesday"
            "TimeSlots@odata.type" = "#Collection(microsoft.graph.bookingWorkTimeSlot)"
            TimeSlots = @(
                @{
                    "@odata.type" = "#microsoft.graph.bookingWorkTimeSlot"
                    End = "17:00:00.0000000"
                    Start = "08:00:00.0000000"
                }
            )
        }
        @{
            "@odata.type" = "#microsoft.graph.bookingWorkHours"
            "Day@odata.type" = "#microsoft.graph.dayOfWeek"
            Day = "wednesday"
            "TimeSlots@odata.type" = "#Collection(microsoft.graph.bookingWorkTimeSlot)"
            TimeSlots = @(
                @{
                    "@odata.type" = "#microsoft.graph.bookingWorkTimeSlot"
                    End = "17:00:00.0000000"
                    Start = "08:00:00.0000000"
                }
            )
        }
        @{
            "@odata.type" = "#microsoft.graph.bookingWorkHours"
            "Day@odata.type" = "#microsoft.graph.dayOfWeek"
            Day = "thursday"
            "TimeSlots@odata.type" = "#Collection(microsoft.graph.bookingWorkTimeSlot)"
            TimeSlots = @(
                @{
                    "@odata.type" = "#microsoft.graph.bookingWorkTimeSlot"
                    End = "17:00:00.0000000"
                    Start = "08:00:00.0000000"
                }
            )
        }
        @{
            "@odata.type" = "#microsoft.graph.bookingWorkHours"
            "Day@odata.type" = "#microsoft.graph.dayOfWeek"
            Day = "friday"
            "TimeSlots@odata.type" = "#Collection(microsoft.graph.bookingWorkTimeSlot)"
            TimeSlots = @(
                @{
                    "@odata.type" = "#microsoft.graph.bookingWorkTimeSlot"
                    End = "17:00:00.0000000"
                    Start = "08:00:00.0000000"
                }
            )
        }
    )
    IsEmailNotificationEnabled = $false
}

New-MgBookingBusinessStaffMember -BookingBusinessId $bookingBusinessId -BodyParameter $params

```