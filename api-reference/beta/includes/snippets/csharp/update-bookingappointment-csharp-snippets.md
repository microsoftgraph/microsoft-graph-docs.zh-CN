---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f89a916c3ade122cd0de532f2aa4b407155b2fa2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35500524"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingAppointment = new BookingAppointment
{
    End = new DateTimeTimeZone
    {
        DateTime = "2018-05-06T15:30:00+03:00",
        TimeZone = "UTC"
    },
    InvoiceDate = new DateTimeTimeZone
    {
        DateTime = "2018-05-06T15:30:00+03:00",
        TimeZone = "UTC"
    },
    Start = new DateTimeTimeZone
    {
        DateTime = "2018-05-06T15:00:00+03:00",
        TimeZone = "UTC"
    }
};

await graphClient.BookingBusinesses["Contosolunchdelivery@M365B489948.onmicrosoft.com"].Appointments["AAMkADKnAAA="]
    .Request()
    .UpdateAsync(bookingAppointment);

```