---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 38de52fa7a3e58142ea81d67e74d498b0e7ac79c
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412750"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/beta/policies/claimsMappingPolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9",
}
options := &msgraphsdk.ClaimsMappingPolicyRequestBuilderPostOptions{
    Body: requestBody,
}
servicePrincipalId := "servicePrincipal-id"
claimsMappingPolicyId := "claimsMappingPolicy-id"
graphClient.ServicePrincipalsById(&servicePrincipalId).ClaimsMappingPoliciesById(&claimsMappingPolicyId).Post(options)


```