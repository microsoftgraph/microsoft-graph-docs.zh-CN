---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d7931f490b3aa8dad4d39ce36f7de5bf820b34c7956375ec6b4c7d56922d3d39
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219980"
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