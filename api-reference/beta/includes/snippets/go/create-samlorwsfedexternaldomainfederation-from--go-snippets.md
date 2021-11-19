---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3f544285f47613d1380a18c208e9c2547a1cf053
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092292"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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