---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b6c33df63f5c50fa53b0899af6ccc0597c47a41
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566709"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityProvider = new OpenIdConnectProvider
{
    Name = "Login with the Contoso identity provider",
    Type = "OpenIDConnect",
    ClientId = "56433757-cadd-4135-8431-2c9e3fd68ae8",
    ClientSecret = "12345",
    ClaimsMapping = new ClaimsMapping
    {
        UserId = "myUserId",
        GivenName = "myGivenName",
        Surname = "mySurname",
        Email = "myEmail",
        DisplayName = "myDisplayName"
    },
    DomainHint = "mycustomoidc",
    MetadataUrl = "https://mycustomoidc.com/.well-known/openid-configuration",
    ResponseMode = OpenIdConnectResponseMode.Form_post,
    ResponseType = OpenIdConnectResponseTypes.Code,
    Scope = "openid"
};

await graphClient.IdentityProviders
    .Request()
    .AddAsync(identityProvider);

```