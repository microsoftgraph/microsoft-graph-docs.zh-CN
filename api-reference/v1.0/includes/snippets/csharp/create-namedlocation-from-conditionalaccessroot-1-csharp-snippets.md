---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d53854c0747a775e772d66d9003b7c289db29c69
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963961"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var namedLocation = new IpNamedLocation
{
    DisplayName = "Untrusted IP named location",
    IsTrusted = false,
    IpRanges = new List<IpRange>()
    {
        new IPv4CidrRange
        {
            CidrAddress = "12.34.221.11/22"
        },
        new IPv6CidrRange
        {
            CidrAddress = "2001:0:9d38:90d6:0:0:0:0/63"
        }
    }
};

await graphClient.Identity.ConditionalAccess.NamedLocations
    .Request()
    .AddAsync(namedLocation);

```