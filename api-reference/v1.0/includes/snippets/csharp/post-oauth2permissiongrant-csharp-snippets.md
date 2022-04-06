---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c6e18a4922e9b8f2cf6dc2d3edc1ddad360ad13a
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758953"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var oAuth2PermissionGrant = new OAuth2PermissionGrant
{
    ClientId = "ef969797-201d-4f6b-960c-e9ed5f31dab5",
    ConsentType = "AllPrincipals",
    ResourceId = "943603e4-e787-4fe9-93d1-e30f749aae39",
    Scope = "DelegatedPermissionGrant.ReadWrite.All"
};

await graphClient.Oauth2PermissionGrants
    .Request()
    .AddAsync(oAuth2PermissionGrant);

```