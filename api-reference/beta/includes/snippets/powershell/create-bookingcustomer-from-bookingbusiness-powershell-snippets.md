---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4546d21a3ad623df4e607de320f2559f106a01e7
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62094652"
---
```powershell

Import-Module Microsoft.Graph.Bookings

$params = @{
    DisplayName = "Joni Sherman"
    EmailAddress = "jonis@relecloud.com"
    Addresses = @(
        @{
            PostOfficeBox = ""
            Street = "4567 Main Street"
            City = "Buffalo"
            State = "NY"
            CountryOrRegion = "USA"
            PostalCode = "98052"
            Type = "home"
        }
        @{
            PostOfficeBox = ""
            Street = "4570 Main Street"
            City = "Buffalo"
            State = "NY"
            CountryOrRegion = "USA"
            PostalCode = "98054"
            Type = "business"
        }
    )
    Phones = @(
        @{
            Number = "206-555-0100"
            Type = "home"
        }
        @{
            Number = "206-555-0200"
            Type = "business"
        }
    )
}

New-MgBookingBusinessCustomer -BookingBusinessId $bookingBusinessId -BodyParameter $params

```