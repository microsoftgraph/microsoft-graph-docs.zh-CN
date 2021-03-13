---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1dff9c5fbc6fd2d72483fc16cf7daab1bf8d0fe1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804499"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.PrivilegedRoleAssignmentRequests["{privilegedRoleAssignmentRequest-id}"]
    .Cancel()
    .Request()
    .PostAsync();

```