---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8e5672ebbabd4b7316c44f640dcf36b67f3e5234
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088587"
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
options := &msgraphsdk.StaffMembersRequestBuilderPostOptions{
    Body: requestBody,
}
bookingBusinessId := "bookingBusiness-id"
result, err := graphClient.BookingBusinessesById(&bookingBusinessId).StaffMembers().Post(options)


```