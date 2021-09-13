---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a2f050bf9f9d9d81e420940249db7b539cad22c67c6d4b0510428315852492b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221419"
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

await graphClient.Identity.ConditionalAccess.NamedLocations["{namedLocation-id}"]
    .Request()
    .UpdateAsync(namedLocation);

```