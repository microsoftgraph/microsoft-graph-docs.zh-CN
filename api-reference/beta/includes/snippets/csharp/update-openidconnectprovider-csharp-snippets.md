---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 09f9696cdb1776bf1f018ecddab6762a1c3b385f
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566671"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityProvider = new IdentityProvider
{
    ResponseType = OpenIdConnectResponseTypes.Id_token
};

await graphClient.IdentityProviders["OIDC-V1-MyTest-085a8a0c-58cb-4b6d-8e07-1328ea404e1a"]
    .Request()
    .UpdateAsync(identityProvider);

```