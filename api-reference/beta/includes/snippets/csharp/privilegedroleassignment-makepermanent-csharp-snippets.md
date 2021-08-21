---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7c2debbfd3d6a3bd034cb9333bfb462b51f98117f05c61bf85974649dcba8cba
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273944"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var reason = "reason-value";

var ticketNumber = "ticketNumber-value";

var ticketSystem = "ticketSystem-value";

await graphClient.PrivilegedRoleAssignments["{privilegedRoleAssignment-id}"]
    .MakePermanent(reason,ticketNumber,ticketSystem)
    .Request()
    .PostAsync();

```