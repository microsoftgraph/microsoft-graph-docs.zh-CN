---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d9dd661491e3552491ce53843297663307a36ca3
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326395"
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
bookingBusinessId := "bookingBusiness-id"
bookingAppointmentId := "bookingAppointment-id"
graphClient.BookingBusinessesById(&bookingBusinessId).AppointmentsById(&bookingAppointmentId).Patch(requestBody)


```