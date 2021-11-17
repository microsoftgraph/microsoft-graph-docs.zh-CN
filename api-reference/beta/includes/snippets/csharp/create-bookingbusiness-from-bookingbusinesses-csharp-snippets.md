---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8bf4668973fded9d05c33c351e45637e47e4b7eda8d05ca12bffedeab9cd35f9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105046"
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