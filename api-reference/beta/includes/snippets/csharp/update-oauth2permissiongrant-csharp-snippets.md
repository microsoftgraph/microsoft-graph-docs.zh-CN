---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d40d4c10eb0f7e15c86a2502fd151863dc8e3207daab65018f15ed2345d7bfb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158508"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var oAuth2PermissionGrant = new OAuth2PermissionGrant
{
    Scope = "scope-value"
};

await graphClient.Oauth2PermissionGrants["{oAuth2PermissionGrant-id}"]
    .Request()
    .UpdateAsync(oAuth2PermissionGrant);

```