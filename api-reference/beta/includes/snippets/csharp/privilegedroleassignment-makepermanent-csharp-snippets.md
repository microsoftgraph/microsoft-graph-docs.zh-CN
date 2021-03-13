---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d75826fbac81ef3502446f89715d53671a98a69d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803254"
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