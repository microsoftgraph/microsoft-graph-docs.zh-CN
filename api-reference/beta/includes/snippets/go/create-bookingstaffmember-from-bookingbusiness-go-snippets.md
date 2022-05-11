---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5375e6688af6d7d99d034d6e0910efc7df31d156
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325957"
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
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.bookingWorkHours",
        "day@odata.type": "#microsoft.graph.dayOfWeek",
        "day": "monday",
        "timeSlots@odata.type": "#Collection(microsoft.graph.bookingWorkTimeSlot)",
        "timeSlots":  []Object {
        }
    }
    msgraphsdk.NewBookingWorkHours(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.bookingWorkHours",
        "day@odata.type": "#microsoft.graph.dayOfWeek",
        "day": "tuesday",
        "timeSlots@odata.type": "#Collection(microsoft.graph.bookingWorkTimeSlot)",
        "timeSlots":  []Object {
        }
    }
    msgraphsdk.NewBookingWorkHours(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.bookingWorkHours",
        "day@odata.type": "#microsoft.graph.dayOfWeek",
        "day": "wednesday",
        "timeSlots@odata.type": "#Collection(microsoft.graph.bookingWorkTimeSlot)",
        "timeSlots":  []Object {
        }
    }
    msgraphsdk.NewBookingWorkHours(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.bookingWorkHours",
        "day@odata.type": "#microsoft.graph.dayOfWeek",
        "day": "thursday",
        "timeSlots@odata.type": "#Collection(microsoft.graph.bookingWorkTimeSlot)",
        "timeSlots":  []Object {
        }
    }
    msgraphsdk.NewBookingWorkHours(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.bookingWorkHours",
        "day@odata.type": "#microsoft.graph.dayOfWeek",
        "day": "friday",
        "timeSlots@odata.type": "#Collection(microsoft.graph.bookingWorkTimeSlot)",
        "timeSlots":  []Object {
        }
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