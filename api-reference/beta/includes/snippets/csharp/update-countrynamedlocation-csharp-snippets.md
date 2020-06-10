---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ed7922f83b6ca480e80cfc1e88e34afd913fc3a
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681115"
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

await graphClient.Identity.ConditionalAccess.NamedLocations["1c4427fd-0885-4a3d-8b23-09a899ffa959"]
    .Request()
    .UpdateAsync(namedLocation);

```