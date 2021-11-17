---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 091657710fb1fab90ced1b3241a8521bf2b8bfafe996746ff8b8ccb0c50401ed
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105532"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workPosition = new WorkPosition
{
    Detail = new PositionDetail
    {
        Company = new CompanyDetail
        {
            DisplayName = "Adventureworks Ltd.",
            Department = "Consulting",
            OfficeLocation = "AW23/344",
            Address = new PhysicalAddress
            {
                Type = PhysicalAddressType.Business,
                Street = "123 Patriachy Ponds",
                City = "Moscow",
                CountryOrRegion = "Russian Federation",
                PostalCode = "RU-34621"
            },
            WebUrl = "https://www.adventureworks.com"
        },
        JobTitle = "Senior Product Branding Manager II",
        Role = "consulting"
    },
    IsCurrent = true
};

await graphClient.Me.Profile.Positions
    .Request()
    .AddAsync(workPosition);

```