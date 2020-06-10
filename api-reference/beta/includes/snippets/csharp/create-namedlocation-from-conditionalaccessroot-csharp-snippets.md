---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: edc31e603c1d0efa700dc5b882c3e77d3b4de66e
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681557"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var namedLocation = new CountryNamedLocation
{
    DisplayName = "Named location with unknown countries and regions",
    CountriesAndRegions = new List<String>()
    {
        "US",
        "GB"
    },
    IncludeUnknownCountriesAndRegions = true
};

await graphClient.Identity.ConditionalAccess.NamedLocations
    .Request()
    .AddAsync(namedLocation);

```