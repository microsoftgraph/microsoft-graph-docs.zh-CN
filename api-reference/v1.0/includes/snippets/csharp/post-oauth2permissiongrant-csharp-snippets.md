---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 689bd562b1a3b89bfb1759e44ddea5ead2764ac1d808ac4e1b442a6643b833cc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277498"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var oAuth2PermissionGrant = new OAuth2PermissionGrant
{
    ClientId = "clientId-value",
    ConsentType = "consentType-value",
    PrincipalId = "principalId-value",
    ResourceId = "resourceId-value",
    Scope = "scope-value"
};

await graphClient.Oauth2PermissionGrants
    .Request()
    .AddAsync(oAuth2PermissionGrant);

```