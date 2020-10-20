---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8d52edd3457689c6ed4011da8008b38c2f1622e5
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48613649"
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