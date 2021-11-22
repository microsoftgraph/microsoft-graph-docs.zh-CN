---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e62b4999d4ea764d1f20f6b90f60d10a2d6f1b7a63f4cd05b04156f93a97c62e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220330"
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