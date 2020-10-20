---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e6743364a59f35d966e2c04814ec3ed77b2e4b6
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48621602"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingBusiness = new BookingBusiness
{
    DisplayName = "Fourth Coffee",
    Address = new PhysicalAddress
    {
        Type = PhysicalAddressType.Unknown,
        PostOfficeBox = "P.O. Box 123",
        Street = "4567 Main Street",
        City = "Buffalo",
        State = "NY",
        CountryOrRegion = "USA",
        PostalCode = "98052"
    },
    Phone = "206-555-0100",
    Email = "manager@fourthcoffee.com",
    WebSiteUrl = "https://www.fourthcoffee.com",
    DefaultCurrencyIso = "USD"
};

await graphClient.BookingBusinesses
    .Request()
    .AddAsync(bookingBusiness);

```