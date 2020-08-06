---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9c7c7c8a63ec29a4d9928ee44e44210ead140a7d
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46567344"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var namedLocation = new IpNamedLocation
{
    DisplayName = "Untrusted named location with only IPv4 address",
    IsTrusted = false,
    IpRanges = new List<IpRange>()
    {
        new IPv4CidrRange
        {
            CidrAddress = "6.5.4.3/18"
        }
    }
};

await graphClient.Identity.ConditionalAccess.NamedLocations["0854951d-5fc0-4eb1-b392-9b2c9d7949c2"]
    .Request()
    .UpdateAsync(namedLocation);

```