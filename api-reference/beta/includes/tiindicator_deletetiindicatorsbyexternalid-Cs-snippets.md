---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 189b925094f47910764415b4b8f03a55de894ce1
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34469291"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var value = new List<String>()
{
    "externalId-value1",
    "externalId-value2"
};

await graphClient.Security.TiIndicators
    .DeleteTiIndicatorsByExternalId(value)
    .Request()
    .PostAsync();

```