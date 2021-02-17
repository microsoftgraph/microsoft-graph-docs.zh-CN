---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1dfea73cfd4426e9cdc097ee95059f8ca582ba3f
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272313"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var rosterPlans = await graphClient.Users["{usersId}"].Planner.RosterPlans
    .Request()
    .GetAsync();

```