---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f7461871d195d482091afa1bc3acc2a96ea3e9b8
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62094842"
---
```powershell

Import-Module Microsoft.Graph.Bookings

$params = @{
    "@odata.type" = "#microsoft.graph.bookingAppointment"
    End = @{
        "@odata.type" = "#microsoft.graph.dateTimeTimeZone"
        DateTime = "2018-05-06T12:30:00.0000000+00:00"
        TimeZone = "UTC"
    }
    InvoiceDate = @{
        "@odata.type" = "#microsoft.graph.dateTimeTimeZone"
        DateTime = "2018-05-06T12:30:00.0000000+00:00"
        TimeZone = "UTC"
    }
    Start = @{
        "@odata.type" = "#microsoft.graph.dateTimeTimeZone"
        DateTime = "2018-05-06T12:00:00.0000000+00:00"
        TimeZone = "UTC"
    }
}

Update-MgBookingBusinessAppointment -BookingBusinessId $bookingBusinessId -BookingAppointmentId $bookingAppointmentId -BodyParameter $params

```