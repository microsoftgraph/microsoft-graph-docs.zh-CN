---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 186e7f557fd9ffbb94cdb2f5c34f650ec1384d50
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091454"
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
graphClient.BookingBusinessesById(&bookingBusinessId).AppointmentsById(&bookingAppointmentId).Patch(options)


```