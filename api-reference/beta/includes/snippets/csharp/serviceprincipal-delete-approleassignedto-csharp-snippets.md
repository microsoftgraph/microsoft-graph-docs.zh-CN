---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b72df6deefcf972f41fa6bd9d28a0a8a052afab5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804402"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.ServicePrincipals["{servicePrincipal-id}"].AppRoleAssignedTo["{appRoleAssignment-id}"]
    .Request()
    .DeleteAsync();

```