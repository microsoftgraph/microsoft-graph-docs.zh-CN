---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a46815fbb41e5931ad61b9994f523fefa437c670
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810421"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityEnabledOnly = true;

await graphClient.ServicePrincipals["{servicePrincipal-id}"]
    .GetMemberObjects(securityEnabledOnly)
    .Request()
    .PostAsync();

```