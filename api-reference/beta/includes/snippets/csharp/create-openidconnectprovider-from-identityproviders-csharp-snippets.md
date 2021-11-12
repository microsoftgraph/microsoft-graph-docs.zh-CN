---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 69bd26627f1aa02aaa1239dc86fe47e2d96cea753029c0665530f7c5748207e3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333029"
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