---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 67b15ac6bc1707eda88eeb7890ea9a333e01fb3baf408fbbb18fc4490a7421ef
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221300"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var rosterPlans = await graphClient.Users["{user-id}"].Planner.RosterPlans
    .Request()
    .GetAsync();

```