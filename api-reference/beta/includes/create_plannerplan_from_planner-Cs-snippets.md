---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8d52edd3457689c6ed4011da8008b38c2f1622e5
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34439979"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerPlan = new PlannerPlan
{
    Owner = "ebf3b108-5234-4e22-b93d-656d7dae5874",
    Title = "title-value"
};

await graphClient.Planner.Plans
    .Request()
    .AddAsync(plannerPlan);

```