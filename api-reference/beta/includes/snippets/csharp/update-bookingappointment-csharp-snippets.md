---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 84e8ccd39bd688965351d6eae5b4785c55c45b4d
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/03/2019
ms.locfileid: "36174702"
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
        DateTime = "2018-05-06T12:30:00+00:00",
        TimeZone = "UTC"
    },
    InvoiceDate = new DateTimeTimeZone
    {
        AdditionalData = new Dictionary<string, object>()
        {
            {"@odata.type","#microsoft.graph.dateTimeTimeZone"}
        },
        DateTime = "2018-05-06T12:30:00+00:00",
        TimeZone = "UTC"
    },
    Start = new DateTimeTimeZone
    {
        AdditionalData = new Dictionary<string, object>()
        {
            {"@odata.type","#microsoft.graph.dateTimeTimeZone"}
        },
        DateTime = "2018-05-06T12:00:00+00:00",
        TimeZone = "UTC"
    }
};

await graphClient.BookingBusinesses["Contosolunchdelivery@M365B489948.onmicrosoft.com"].Appointments["AAMkADKnAAA="]
    .Request()
    .UpdateAsync(bookingAppointment);

```