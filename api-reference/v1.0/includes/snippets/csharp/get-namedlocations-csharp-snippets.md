---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c36d745fed166c449f761ef15b7b627efe11e461
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566021"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var namedLocations = await graphClient.Identity.ConditionalAccess.NamedLocations
    .Request()
    .Filter("microsoft.graph.countryNamedLocation/countriesAndRegions/any(c: c eq 'CA')")
    .GetAsync();

```