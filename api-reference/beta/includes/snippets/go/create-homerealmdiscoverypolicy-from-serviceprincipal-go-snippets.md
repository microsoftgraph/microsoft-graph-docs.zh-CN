---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2422a17b3235a267886d0a2a0ae2835358dc0218
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412288"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/beta/policies/homeRealmDiscoveryPolicies/6c6f154f-cb39-4ff9-bf5b-62d5ad585cde",
}
options := &msgraphsdk.HomeRealmDiscoveryPolicyRequestBuilderPostOptions{
    Body: requestBody,
}
servicePrincipalId := "servicePrincipal-id"
homeRealmDiscoveryPolicyId := "homeRealmDiscoveryPolicy-id"
graphClient.ServicePrincipalsById(&servicePrincipalId).HomeRealmDiscoveryPoliciesById(&homeRealmDiscoveryPolicyId).Post(options)


```