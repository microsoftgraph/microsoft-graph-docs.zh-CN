---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0d08aa18919c363f008d8e760a56385fd6f2de9830c405cf45ca1332888cdc4c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332482"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var reason = "reason-value";

var duration = "duration-value";

var ticketNumber = "ticketNumber-value";

var ticketSystem = "ticketSystem-value";

await graphClient.PrivilegedRoles["{privilegedRole-id}"]
    .SelfActivate(reason,duration,ticketNumber,ticketSystem)
    .Request()
    .PostAsync();

```