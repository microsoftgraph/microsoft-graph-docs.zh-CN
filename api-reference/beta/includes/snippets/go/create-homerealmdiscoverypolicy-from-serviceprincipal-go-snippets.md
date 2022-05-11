---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 119ac233c0c051abf4cdc460d42665c47d581573
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65329070"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/beta/policies/homeRealmDiscoveryPolicies/6c6f154f-cb39-4ff9-bf5b-62d5ad585cde",
}
servicePrincipalId := "servicePrincipal-id"
homeRealmDiscoveryPolicyId := "homeRealmDiscoveryPolicy-id"
graphClient.ServicePrincipalsById(&servicePrincipalId).HomeRealmDiscoveryPoliciesById(&homeRealmDiscoveryPolicyId).Post(requestBody)


```