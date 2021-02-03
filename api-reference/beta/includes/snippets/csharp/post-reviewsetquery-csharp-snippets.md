---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 61a1d67d504234cd22dde9273efa691035455cff
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2021
ms.locfileid: "50093662"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var reviewSetQuery = new Microsoft.Graph.Ediscovery.ReviewSetQuery
{
    DisplayName = "My Query 1",
    Query = "(subject:\"Quarterly Financials\")"
};

await graphClient.Compliance.Ediscovery.Cases["2eef613a-ca2d-42f4-89fe-84d5198ddedf"].ReviewSets["b26888b3-e1f5-47c5-bdf2-33d1b90cb2e8"].Queries
    .Request()
    .AddAsync(reviewSetQuery);

```