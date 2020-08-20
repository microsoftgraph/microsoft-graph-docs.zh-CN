---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e0bfb2ca3566a8647e1d9638be99bab9e607c1c5
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46820217"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var itemAddress = new ItemAddress
{
    DisplayName = "Home",
    Detail = new PhysicalAddress
    {
        Type = PhysicalAddressType.Home,
        PostOfficeBox = null,
        Street = "221B Baker Street",
        City = "London",
        State = null,
        CountryOrRegion = "United Kingdom",
        PostalCode = "E14 3TD"
    }
};

await graphClient.Me.Profile.Addresses
    .Request()
    .AddAsync(itemAddress);

```