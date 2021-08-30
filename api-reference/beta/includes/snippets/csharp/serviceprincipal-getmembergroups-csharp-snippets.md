---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 67915e903695350e06b70e1ff89633ee9b4d91cd2fdb70d82b5a3f76c1a81b22
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903060"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityEnabledOnly = true;

await graphClient.ServicePrincipals["{servicePrincipal-id}"]
    .GetMemberGroups(securityEnabledOnly)
    .Request()
    .PostAsync();

```