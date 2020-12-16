---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ebd39236355a18eefcd78c8df09e2dc9be5b2464
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49691373"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authorizationPolicy = new AuthorizationPolicy
{
    AllowEmailVerifiedUsersToJoinOrganization = false
};

await graphClient.Policies.AuthorizationPolicy
    .Request()
    .UpdateAsync(authorizationPolicy);

```