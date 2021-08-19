---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fd0eed1e33cce88a3dd9471d62908e7880f550384497ed1b3dee94e65fc45b84
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162082"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityProviderBase = new OpenIdConnectIdentityProvider
{
    DisplayName = "Login with the Contoso identity provider",
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

await graphClient.Identity.IdentityProviders
    .Request()
    .AddAsync(identityProviderBase);

```