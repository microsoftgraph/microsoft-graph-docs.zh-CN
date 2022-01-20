---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4baa28b676a7de4ad24fef13d4f9a3d5675ad47c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62124092"
---
```powershell

Import-Module Microsoft.Graph.Bookings

$params = @{
    WorkingHours = @(
        @{
            "@odata.type" = "#microsoft.graph.bookingWorkHours"
            "Day@odata.type" = "#microsoft.graph.dayOfWeek"
            Day = "monday"
            "TimeSlots@odata.type" = "#Collection(microsoft.graph.bookingWorkTimeSlot)"
            TimeSlots = @(
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
}

Update-MgBookingBusinessStaffMember -BookingBusinessId $bookingBusinessId -BookingStaffMemberId $bookingStaffMemberId -BodyParameter $params

```