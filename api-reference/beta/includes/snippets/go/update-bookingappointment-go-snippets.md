---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a0a9354d91b2bbb67fc52f749912aeee068455a
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411924"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewBookingAppointment()
end := msgraphsdk.NewDateTimeTimeZone()
requestBody.SetEnd(end)
dateTime := "2018-05-06T12:30:00.0000000+00:00"
end.SetDateTime(&dateTime)
timeZone := "UTC"
end.SetTimeZone(&timeZone)
end.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.dateTimeTimeZone",
}
invoiceDate := msgraphsdk.NewDateTimeTimeZone()
requestBody.SetInvoiceDate(invoiceDate)
dateTime := "2018-05-06T12:30:00.0000000+00:00"
invoiceDate.SetDateTime(&dateTime)
timeZone := "UTC"
invoiceDate.SetTimeZone(&timeZone)
invoiceDate.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.dateTimeTimeZone",
}
start := msgraphsdk.NewDateTimeTimeZone()
requestBody.SetStart(start)
dateTime := "2018-05-06T12:00:00.0000000+00:00"
start.SetDateTime(&dateTime)
timeZone := "UTC"
start.SetTimeZone(&timeZone)
start.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.dateTimeTimeZone",
}
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.bookingAppointment",
}
options := &msgraphsdk.BookingAppointmentRequestBuilderPatchOptions{
    Body: requestBody,
}
bookingBusinessId := "bookingBusiness-id"
bookingAppointmentId := "bookingAppointment-id"
result, err := graphClient.BookingBusinessesById(&bookingBusinessId).AppointmentsById(&bookingAppointmentId).Patch(options)


```