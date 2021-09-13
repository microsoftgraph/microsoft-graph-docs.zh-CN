---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2bf488e677f57f5c16db5bbf984dc1c43aeae306f43720521fdee83122ddd5a8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332171"
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