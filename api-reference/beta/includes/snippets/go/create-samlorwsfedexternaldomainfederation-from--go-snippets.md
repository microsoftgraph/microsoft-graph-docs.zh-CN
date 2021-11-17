---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7544ac6f56f139c38636fcccc3fa037df4e59111
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61002693"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewIdentityProviderBase()
displayName := "contoso display name"
requestBody.SetDisplayName(&displayName)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.samlOrWsFedExternalDomainFederation",
    "issuerUri": "https://contoso.com/issuerUri",
    "metadataExchangeUri": "https://contoso.com/metadataExchangeUri",
    "passiveSignInUri": "https://contoso.com/signin",
    "preferredAuthenticationProtocol": "wsFed",
    "domains":  []Object {
    }
    "signingCertificate": "MIIDADCCAeigAwIBAgIQEX41y8r6",
}
options := &msgraphsdk.FederationConfigurationsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Directory().FederationConfigurations().Post(options)


```