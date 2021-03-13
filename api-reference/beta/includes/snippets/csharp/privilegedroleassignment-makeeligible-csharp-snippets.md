---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2bf50b1802106ce7cc8e8543d4f728a3d56e79f0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805333"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.PrivilegedRoleAssignments["{privilegedRoleAssignment-id}"]
    .MakeEligible()
    .Request()
    .PostAsync();

```