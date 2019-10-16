---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 88e48c86f53a8accb344cd3a50a2a414795957b3
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37544181"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingAppointment = new BookingAppointment
{
    End = new DateTimeTimeZone
    {
        DateTime = "2018-05-06T12:30:00+00:00",
        TimeZone = "UTC"
    },
    InvoiceDate = new DateTimeTimeZone
    {
        DateTime = "2018-05-06T12:30:00+00:00",
        TimeZone = "UTC"
    },
    Start = new DateTimeTimeZone
    {
        DateTime = "2018-05-06T12:00:00+00:00",
        TimeZone = "UTC"
    }
};

await graphClient.BookingBusinesses["Contosolunchdelivery@M365B489948.onmicrosoft.com"].Appointments["AAMkADKnAAA="]
    .Request()
    .UpdateAsync(bookingAppointment);

```