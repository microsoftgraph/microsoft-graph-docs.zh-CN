---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 31a630b549ad081bab43959f6da709f570526f7b
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202363"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    "@odata.type" = "#microsoft.graph.internalDomainFederation"
    DisplayName = "Contoso"
    IssuerUri = "http://contoso.com/adfs/services/trust"
    MetadataExchangeUri = "https://sts.contoso.com/adfs/services/trust/mex"
    SigningCertificate = "MIIE3jCCAsagAwIBAgIQQcyDaZz3MI"
    PassiveSignInUri = "https://sts.contoso.com/adfs/ls"
    PreferredAuthenticationProtocol = "wsFed"
    ActiveSignInUri = "https://sts.contoso.com/adfs/services/trust/2005/usernamemixed"
    SignOutUri = "https://sts.contoso.com/adfs/ls"
    PromptLoginBehavior = "nativeSupport"
    IsSignedAuthenticationRequestRequired = $true
    NextSigningCertificate = "MIIE3jCCAsagAwIBAgIQQcyDaZz3MI"
    FederatedIdpMfaBehavior = "rejectMfaByFederatedIdp"
}

New-MgDomainFederationConfiguration -DomainId $domainId -BodyParameter $params

```