---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 387cd0de676991fe2e4090c426b6f685b24397e1
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/03/2019
ms.locfileid: "36174705"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingAppointment bookingAppointment = new BookingAppointment();
bookingAppointment.additionalDataManager().put("@odata.type", new JsonPrimitive("#microsoft.graph.bookingAppointment"));
DateTimeTimeZone end = new DateTimeTimeZone();
end.additionalDataManager().put("@odata.type", new JsonPrimitive("#microsoft.graph.dateTimeTimeZone"));
end.dateTime = "2018-05-06T12:30:00+00:00";
end.timeZone = "UTC";
bookingAppointment.end = end;
DateTimeTimeZone invoiceDate = new DateTimeTimeZone();
invoiceDate.additionalDataManager().put("@odata.type", new JsonPrimitive("#microsoft.graph.dateTimeTimeZone"));
invoiceDate.dateTime = "2018-05-06T12:30:00+00:00";
invoiceDate.timeZone = "UTC";
bookingAppointment.invoiceDate = invoiceDate;
DateTimeTimeZone start = new DateTimeTimeZone();
start.additionalDataManager().put("@odata.type", new JsonPrimitive("#microsoft.graph.dateTimeTimeZone"));
start.dateTime = "2018-05-06T12:00:00+00:00";
start.timeZone = "UTC";
bookingAppointment.start = start;

graphClient.bookingBusinesses("Contosolunchdelivery@M365B489948.onmicrosoft.com").appointments("AAMkADKnAAA=")
    .buildRequest()
    .patch(bookingAppointment);

```