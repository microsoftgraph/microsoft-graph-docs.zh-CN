---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5bc3c19ec44db351f7994f056a1250f613b70885
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61003476"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewBookingBusiness()
email := "admin@fabrikam.com"
requestBody.SetEmail(&email)
schedulingPolicy := msgraphsdk.NewBookingSchedulingPolicy()
requestBody.SetSchedulingPolicy(schedulingPolicy)
timeSlotInterval := "PT60M"
schedulingPolicy.SetTimeSlotInterval(&timeSlotInterval)
minimumLeadTime := "P1D"
schedulingPolicy.SetMinimumLeadTime(&minimumLeadTime)
maximumAdvance := "P30D"
schedulingPolicy.SetMaximumAdvance(&maximumAdvance)
sendConfirmationsToOwner := true
schedulingPolicy.SetSendConfirmationsToOwner(&sendConfirmationsToOwner)
allowStaffSelection := true
schedulingPolicy.SetAllowStaffSelection(&allowStaffSelection)
options := &msgraphsdk.BookingBusinessRequestBuilderPatchOptions{
    Body: requestBody,
}
bookingBusinessId := "bookingBusiness-id"
graphClient.BookingBusinessesById(&bookingBusinessId).Patch(options)


```