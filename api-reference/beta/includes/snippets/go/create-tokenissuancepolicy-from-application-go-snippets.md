---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4fb58c56a78b6bec3c94df542059942d2b793fcc
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326301"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/beta/policies/tokenIssuancePolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9",
}
applicationId := "application-id"
tokenIssuancePolicyId := "tokenIssuancePolicy-id"
graphClient.ApplicationsById(&applicationId).TokenIssuancePoliciesById(&tokenIssuancePolicyId).Post(requestBody)


```