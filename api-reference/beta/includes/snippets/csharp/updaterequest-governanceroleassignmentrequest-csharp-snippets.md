---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d530647fb0aada1bfff26146775b3ab1b1582e2d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791709"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.PrivilegedAccess["{privilegedAccess-id}"].RoleAssignmentRequests["{governanceRoleAssignmentRequest-id}"]
    .UpdateRequest(null,null,null,null)
    .Request()
    .PostAsync();

```