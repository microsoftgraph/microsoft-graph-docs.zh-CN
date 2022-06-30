---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1296f7577cf624601e58805a7997c51ba91a79e4
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66503170"
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
isEmailNotificationEnabled := false
requestBody.SetIsEmailNotificationEnabled(&isEmailNotificationEnabled)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.bookingStaffMember",
    "role@odata.type": "#microsoft.graph.bookingStaffRole",
    "workingHours@odata.type": "#Collection(microsoft.graph.bookingWorkHours)",
}
bookingBusinessId := "bookingBusiness-id"
result, err := graphClient.BookingBusinessesById(&bookingBusinessId).StaffMembers().Post(requestBody)


```