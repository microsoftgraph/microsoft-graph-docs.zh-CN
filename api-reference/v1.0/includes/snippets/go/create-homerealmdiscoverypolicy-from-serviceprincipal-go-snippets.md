---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dfd2b1992b758b2226547bd9d37c1af588d96806
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326951"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/v1.0/policies/homeRealmDiscoveryPolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9",
}
servicePrincipalId := "servicePrincipal-id"
homeRealmDiscoveryPolicyId := "homeRealmDiscoveryPolicy-id"
graphClient.ServicePrincipalsById(&servicePrincipalId).HomeRealmDiscoveryPoliciesById(&homeRealmDiscoveryPolicyId).Post(requestBody)


```