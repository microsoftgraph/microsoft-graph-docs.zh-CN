---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2110de7a3b1db06defba6fc34078b98015afbc8b
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327978"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewInternalDomainFederation()
displayName := "Contoso name change"
requestBody.SetDisplayName(&displayName)
federatedIdpMfaBehavior := "acceptIfMfaDoneByFederatedIdp"
requestBody.SetFederatedIdpMfaBehavior(&federatedIdpMfaBehavior)
domainId := "domain-id"
internalDomainFederationId := "internalDomainFederation-id"
graphClient.DomainsById(&domainId).FederationConfigurationById(&internalDomainFederationId).Patch(requestBody)


```