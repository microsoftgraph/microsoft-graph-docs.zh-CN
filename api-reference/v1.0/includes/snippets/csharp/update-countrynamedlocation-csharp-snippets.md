---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 84ec437672787bc2637578c43e8cc23d5f844b76
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790430"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var namedLocation = new CountryNamedLocation
{
    DisplayName = "Updated named location without unknown countries and regions",
    CountriesAndRegions = new List<String>()
    {
        "CA",
        "IN"
    },
    IncludeUnknownCountriesAndRegions = false
};

await graphClient.Identity.ConditionalAccess.NamedLocations["{namedLocation-id}"]
    .Request()
    .UpdateAsync(namedLocation);

```