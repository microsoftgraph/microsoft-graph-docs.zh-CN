---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e04a8be2403ec003dc1f12b942c28c15722f682e
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44338952"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var oAuth2PermissionGrant = new OAuth2PermissionGrant
{
    Scope = "scope-value"
};

await graphClient.Oauth2PermissionGrants["{id}"]
    .Request()
    .UpdateAsync(oAuth2PermissionGrant);

```