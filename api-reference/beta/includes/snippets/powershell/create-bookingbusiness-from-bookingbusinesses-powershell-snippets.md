---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 41adf335dfdd001054b7530730cffc8c8169e68e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62094717"
---
```powershell

Import-Module Microsoft.Graph.Bookings

$params = @{
    DisplayName = "Fourth Coffee"
    Address = @{
        Type = "mall"
        PostOfficeBox = "P.O. Box 123"
        Street = "4567 Main Street"
        City = "Buffalo"
        State = "NY"
        CountryOrRegion = "USA"
        PostalCode = "98052"
    }
    Phone = "206-555-0100"
    Email = "manager@fourthcoffee.com"
    WebSiteUrl = "https://www.fourthcoffee.com"
    DefaultCurrencyIso = "USD"
}

New-MgBookingBusiness -BodyParameter $params

```