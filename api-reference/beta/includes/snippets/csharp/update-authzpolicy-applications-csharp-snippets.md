---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9d23f94861fb07eb651ab5485c61bed17648635c310668da752dbb8a612e5c32
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105053"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authorizationPolicy = new AuthorizationPolicy
{
    DefaultUserRolePermissions = new DefaultUserRolePermissions
    {
        AllowedToCreateApps = false
    }
};

await graphClient.Policies.AuthorizationPolicy["{authorizationPolicy-id}"]
    .Request()
    .UpdateAsync(authorizationPolicy);

```