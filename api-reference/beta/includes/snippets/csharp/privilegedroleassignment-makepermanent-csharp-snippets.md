---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 80492e83264120091482df6029cdbb0f8bd8b40f
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48612871"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var reason = "reason-value";

var ticketNumber = "ticketNumber-value";

var ticketSystem = "ticketSystem-value";

await graphClient.PrivilegedRoleAssignments["{id}"]
    .MakePermanent(reason,ticketNumber,ticketSystem)
    .Request()
    .PostAsync();

```