---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d730c390990d1b0bf26773e276bc4f360cf54f62
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202368"
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
options := &msgraphsdk.FederationConfigurationRequestBuilderPostOptions{
    Body: requestBody,
}
domainId := "domain-id"
result, err := graphClient.DomainsById(&domainId).FederationConfiguration().Post(options)


```