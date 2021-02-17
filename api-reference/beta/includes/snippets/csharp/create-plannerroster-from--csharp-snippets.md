---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e4b214c1477ca54764ac32523576aa420f928ca4
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272021"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerRoster = new PlannerRoster
{
};

await graphClient.Planner.Rosters
    .Request()
    .AddAsync(plannerRoster);

```