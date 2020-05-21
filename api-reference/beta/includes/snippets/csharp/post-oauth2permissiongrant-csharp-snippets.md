---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a2f74ebb83a4c7a7dbb12e6a27a0ed484775c53c
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44333677"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var oAuth2PermissionGrant = new OAuth2PermissionGrant
{
    ClientId = "clientId-value",
    ConsentType = "consentType-value",
    PrincipalId = "principalId-value",
    ResourceId = "resourceId-value",
    Scope = "scope-value",
    StartTime = DateTimeOffset.Parse("2016-10-19T10:37:00Z"),
    ExpiryTime = DateTimeOffset.Parse("2016-10-19T10:37:00Z")
};

await graphClient.Oauth2PermissionGrants
    .Request()
    .AddAsync(oAuth2PermissionGrant);

```