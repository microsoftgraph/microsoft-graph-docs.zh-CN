---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4e6743364a59f35d966e2c04814ec3ed77b2e4b6
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34434474"
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