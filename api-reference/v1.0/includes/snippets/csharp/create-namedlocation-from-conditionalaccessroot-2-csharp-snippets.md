---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3e485ee4d9fa21fddf254f3233f19b4965d9e3febc9c922c98ac6cdd647cc557
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279198"
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