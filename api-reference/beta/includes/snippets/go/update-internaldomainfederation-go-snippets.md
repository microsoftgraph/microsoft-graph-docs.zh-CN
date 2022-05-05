---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: da91fe73825b888a2703d2af9f5494ad68d876c0
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211725"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewInternalDomainFederation()
displayName := "Contoso name change"
requestBody.SetDisplayName(&displayName)
federatedIdpMfaBehavior := "acceptIfMfaDoneByFederatedIdp"
requestBody.SetFederatedIdpMfaBehavior(&federatedIdpMfaBehavior)
options := &msgraphsdk.InternalDomainFederationRequestBuilderPatchOptions{
    Body: requestBody,
}
domainId := "domain-id"
internalDomainFederationId := "internalDomainFederation-id"
graphClient.DomainsById(&domainId).FederationConfigurationById(&internalDomainFederationId).Patch(options)


```