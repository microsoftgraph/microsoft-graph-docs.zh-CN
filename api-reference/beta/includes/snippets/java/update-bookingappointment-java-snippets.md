---
description: 自动生成的文件。 不修改
ms.openlocfilehash: db0b052bf9c1927f9c379e260ae4c53052f91e32
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865962"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingAppointment bookingAppointment = new BookingAppointment();
bookingAppointment.additionalDataManager().put("@odata.type", new JsonPrimitive("#microsoft.graph.bookingAppointment"));
DateTimeTimeZone end = new DateTimeTimeZone();
end.additionalDataManager().put("@odata.type", new JsonPrimitive("#microsoft.graph.dateTimeTimeZone"));
end.dateTime = "2018-05-06T15:30:00+03:00";
end.timeZone = "UTC";
bookingAppointment.end = end;
DateTimeTimeZone invoiceDate = new DateTimeTimeZone();
invoiceDate.additionalDataManager().put("@odata.type", new JsonPrimitive("#microsoft.graph.dateTimeTimeZone"));
invoiceDate.dateTime = "2018-05-06T15:30:00+03:00";
invoiceDate.timeZone = "UTC";
bookingAppointment.invoiceDate = invoiceDate;
DateTimeTimeZone start = new DateTimeTimeZone();
start.additionalDataManager().put("@odata.type", new JsonPrimitive("#microsoft.graph.dateTimeTimeZone"));
start.dateTime = "2018-05-06T15:00:00+03:00";
start.timeZone = "UTC";
bookingAppointment.start = start;

graphClient.bookingBusinesses("Contosolunchdelivery@M365B489948.onmicrosoft.com").appointments("AAMkADKnAAA=")
    .buildRequest()
    .patch(bookingAppointment);

```