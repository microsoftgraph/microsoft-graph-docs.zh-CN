---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c79b8f5bb3191b4c42fbc17738b0fd000988ee5
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60736644"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingCustomer = new BookingCustomer
{
    DisplayName = "Joni Sherman",
    EmailAddress = "jonis@relecloud.com",
    Addresses = new List<PhysicalAddress>()
    {
        new PhysicalAddress
        {
            PostOfficeBox = "",
            Street = "4567 Main Street",
            City = "Buffalo",
            State = "NY",
            CountryOrRegion = "USA",
            PostalCode = "98052",
            Type = PhysicalAddressType.Home
        },
        new PhysicalAddress
        {
            PostOfficeBox = "",
            Street = "4570 Main Street",
            City = "Buffalo",
            State = "NY",
            CountryOrRegion = "USA",
            PostalCode = "98054",
            Type = PhysicalAddressType.Business
        }
    },
    Phones = new List<Phone>()
    {
        new Phone
        {
            Number = "206-555-0100",
            Type = PhoneType.Home
        },
        new Phone
        {
            Number = "206-555-0200",
            Type = PhoneType.Business
        }
    }
};

await graphClient.BookingBusinesses["{bookingBusiness-id}"].Customers
    .Request()
    .AddAsync(bookingCustomer);

```