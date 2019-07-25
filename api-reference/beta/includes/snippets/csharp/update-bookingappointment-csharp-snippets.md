---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 111196470cb8727425e2dc22cef0a75f45fe18c9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865963"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingAppointment = new BookingAppointment
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.type","#microsoft.graph.bookingAppointment"}
    },
    End = new DateTimeTimeZone
    {
        AdditionalData = new Dictionary<string, object>()
        {
            {"@odata.type","#microsoft.graph.dateTimeTimeZone"}
        },
        DateTime = "2018-05-06T15:30:00+03:00",
        TimeZone = "UTC"
    },
    InvoiceDate = new DateTimeTimeZone
    {
        AdditionalData = new Dictionary<string, object>()
        {
            {"@odata.type","#microsoft.graph.dateTimeTimeZone"}
        },
        DateTime = "2018-05-06T15:30:00+03:00",
        TimeZone = "UTC"
    },
    Start = new DateTimeTimeZone
    {
        AdditionalData = new Dictionary<string, object>()
        {
            {"@odata.type","#microsoft.graph.dateTimeTimeZone"}
        },
        DateTime = "2018-05-06T15:00:00+03:00",
        TimeZone = "UTC"
    }
};

await graphClient.BookingBusinesses["Contosolunchdelivery@M365B489948.onmicrosoft.com"].Appointments["AAMkADKnAAA="]
    .Request()
    .UpdateAsync(bookingAppointment);

```