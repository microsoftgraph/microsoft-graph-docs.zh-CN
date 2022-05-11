---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c5579df165615aa7d169ac0def459f4ffba034c9
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327715"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewInternalDomainFederation()
displayName := "Contoso"
requestBody.SetDisplayName(&displayName)
issuerUri := "http://contoso.com/adfs/services/trust"
requestBody.SetIssuerUri(&issuerUri)
metadataExchangeUri := "https://sts.contoso.com/adfs/services/trust/mex"
requestBody.SetMetadataExchangeUri(&metadataExchangeUri)
signingCertificate := "MIIE3jCCAsagAwIBAgIQQcyDaZz3MI"
requestBody.SetSigningCertificate(&signingCertificate)
passiveSignInUri := "https://sts.contoso.com/adfs/ls"
requestBody.SetPassiveSignInUri(&passiveSignInUri)
preferredAuthenticationProtocol := "wsFed"
requestBody.SetPreferredAuthenticationProtocol(&preferredAuthenticationProtocol)
activeSignInUri := "https://sts.contoso.com/adfs/services/trust/2005/usernamemixed"
requestBody.SetActiveSignInUri(&activeSignInUri)
signOutUri := "https://sts.contoso.com/adfs/ls"
requestBody.SetSignOutUri(&signOutUri)
promptLoginBehavior := "nativeSupport"
requestBody.SetPromptLoginBehavior(&promptLoginBehavior)
isSignedAuthenticationRequestRequired := true
requestBody.SetIsSignedAuthenticationRequestRequired(&isSignedAuthenticationRequestRequired)
nextSigningCertificate := "MIIE3jCCAsagAwIBAgIQQcyDaZz3MI"
requestBody.SetNextSigningCertificate(&nextSigningCertificate)
federatedIdpMfaBehavior := "rejectMfaByFederatedIdp"
requestBody.SetFederatedIdpMfaBehavior(&federatedIdpMfaBehavior)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.internalDomainFederation",
}
domainId := "domain-id"
result, err := graphClient.DomainsById(&domainId).FederationConfiguration().Post(requestBody)


```