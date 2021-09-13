---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b5dfc846c9976cb97ff843be05527db229a557beb2b6e2c1862066218066f46d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333729"
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