---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8d52edd3457689c6ed4011da8008b38c2f1622e5
ms.sourcegitcommit: d8a425766aa6a56027b8576bbec6a9d1ae3e079c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2019
ms.locfileid: "35723007"
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