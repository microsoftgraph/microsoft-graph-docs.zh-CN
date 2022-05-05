---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6e7f05323a4e971c95c935e02da4575d0dc5cd09
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202362"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var internalDomainFederation = new InternalDomainFederation
{
    DisplayName = "Contoso",
    IssuerUri = "http://contoso.com/adfs/services/trust",
    MetadataExchangeUri = "https://sts.contoso.com/adfs/services/trust/mex",
    SigningCertificate = "MIIE3jCCAsagAwIBAgIQQcyDaZz3MI",
    PassiveSignInUri = "https://sts.contoso.com/adfs/ls",
    PreferredAuthenticationProtocol = AuthenticationProtocol.WsFed,
    ActiveSignInUri = "https://sts.contoso.com/adfs/services/trust/2005/usernamemixed",
    SignOutUri = "https://sts.contoso.com/adfs/ls",
    PromptLoginBehavior = PromptLoginBehavior.NativeSupport,
    IsSignedAuthenticationRequestRequired = true,
    NextSigningCertificate = "MIIE3jCCAsagAwIBAgIQQcyDaZz3MI",
    FederatedIdpMfaBehavior = FederatedIdpMfaBehavior.RejectMfaByFederatedIdp
};

await graphClient.Domains["{domain-id}"].FederationConfiguration
    .Request()
    .AddAsync(internalDomainFederation);

```