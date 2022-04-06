---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a1338d71ec6e12c29cdfe0f27e88c524670a5ff
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758759"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var oAuth2PermissionGrant = new OAuth2PermissionGrant
{
    ClientId = "ef969797-201d-4f6b-960c-e9ed5f31dab5",
    ConsentType = "AllPrincipals",
    ResourceId = "943603e4-e787-4fe9-93d1-e30f749aae39",
    Scope = "DelegatedPermissionGrant.ReadWrite.All",
    StartTime = DateTimeOffset.Parse("2022-03-17T00:00:00Z"),
    ExpiryTime = DateTimeOffset.Parse("2023-03-17T00:00:00Z")
};

await graphClient.Oauth2PermissionGrants
    .Request()
    .AddAsync(oAuth2PermissionGrant);

```