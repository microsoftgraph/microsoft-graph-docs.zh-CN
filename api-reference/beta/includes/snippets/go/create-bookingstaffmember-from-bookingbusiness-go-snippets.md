---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 909ff5e092f6d1968dcf0b4cbf043e3f0288bf88
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098749"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewBookingStaffMember()
colorIndex := int32(1)
requestBody.SetColorIndex(&colorIndex)
displayName := "Dana Swope"
requestBody.SetDisplayName(&displayName)
emailAddress := "danas@contoso.com"
requestBody.SetEmailAddress(&emailAddress)
role := "externalGuest"
requestBody.SetRole(&role)
timeZone := "America/Chicago"
requestBody.SetTimeZone(&timeZone)
useBusinessHours := true
requestBody.SetUseBusinessHours(&useBusinessHours)
requestBody.SetWorkingHours( []BookingWorkHours {
    msgraphsdk.NewBookingWorkHours(),
day := "monday"
    SetDay(&day)
    SetTimeSlots( []BookingWorkTimeSlot {
        msgraphsdk.NewBookingWorkTimeSlot(),
end := "17:00:00.0000000"
        SetEnd(&end)
start := "08:00:00.0000000"
        SetStart(&start)
        SetAdditionalData(map[string]interface{}{
            "@odata.type": "#microsoft.graph.bookingWorkTimeSlot",
        }
    }
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.bookingWorkHours",
        "day@odata.type": "#microsoft.graph.dayOfWeek",
        "timeSlots@odata.type": "#Collection(microsoft.graph.bookingWorkTimeSlot)",
    }
    msgraphsdk.NewBookingWorkHours(),
day := "tuesday"
    SetDay(&day)
    SetTimeSlots( []BookingWorkTimeSlot {
        msgraphsdk.NewBookingWorkTimeSlot(),
end := "17:00:00.0000000"
        SetEnd(&end)
start := "08:00:00.0000000"
        SetStart(&start)
        SetAdditionalData(map[string]interface{}{
            "@odata.type": "#microsoft.graph.bookingWorkTimeSlot",
        }
    }
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.bookingWorkHours",
        "day@odata.type": "#microsoft.graph.dayOfWeek",
        "timeSlots@odata.type": "#Collection(microsoft.graph.bookingWorkTimeSlot)",
    }
    msgraphsdk.NewBookingWorkHours(),
day := "wednesday"
    SetDay(&day)
    SetTimeSlots( []BookingWorkTimeSlot {
        msgraphsdk.NewBookingWorkTimeSlot(),
end := "17:00:00.0000000"
        SetEnd(&end)
start := "08:00:00.0000000"
        SetStart(&start)
        SetAdditionalData(map[string]interface{}{
            "@odata.type": "#microsoft.graph.bookingWorkTimeSlot",
        }
    }
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.bookingWorkHours",
        "day@odata.type": "#microsoft.graph.dayOfWeek",
        "timeSlots@odata.type": "#Collection(microsoft.graph.bookingWorkTimeSlot)",
    }
    msgraphsdk.NewBookingWorkHours(),
day := "thursday"
    SetDay(&day)
    SetTimeSlots( []BookingWorkTimeSlot {
        msgraphsdk.NewBookingWorkTimeSlot(),
end := "17:00:00.0000000"
        SetEnd(&end)
start := "08:00:00.0000000"
        SetStart(&start)
        SetAdditionalData(map[string]interface{}{
            "@odata.type": "#microsoft.graph.bookingWorkTimeSlot",
        }
    }
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.bookingWorkHours",
        "day@odata.type": "#microsoft.graph.dayOfWeek",
        "timeSlots@odata.type": "#Collection(microsoft.graph.bookingWorkTimeSlot)",
    }
    msgraphsdk.NewBookingWorkHours(),
day := "friday"
    SetDay(&day)
    SetTimeSlots( []BookingWorkTimeSlot {
        msgraphsdk.NewBookingWorkTimeSlot(),
end := "17:00:00.0000000"
        SetEnd(&end)
start := "08:00:00.0000000"
        SetStart(&start)
        SetAdditionalData(map[string]interface{}{
            "@odata.type": "#microsoft.graph.bookingWorkTimeSlot",
        }
    }
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.bookingWorkHours",
        "day@odata.type": "#microsoft.graph.dayOfWeek",
        "timeSlots@odata.type": "#Collection(microsoft.graph.bookingWorkTimeSlot)",
    }
}
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.bookingStaffMember",
    "role@odata.type": "#microsoft.graph.bookingStaffRole",
    "workingHours@odata.type": "#Collection(microsoft.graph.bookingWorkHours)",
}
bookingBusinessId := "bookingBusiness-id"
result, err := graphClient.BookingBusinessesById(&bookingBusinessId).StaffMembers().Post(requestBody)


```