---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1564153ce93ddd2cc71c24bed1bf07a98a2efb13
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327244"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/v1.0/policies/tokenLifetimePolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9",
}
applicationId := "application-id"
tokenLifetimePolicyId := "tokenLifetimePolicy-id"
graphClient.ApplicationsById(&applicationId).TokenLifetimePoliciesById(&tokenLifetimePolicyId).Post(requestBody)


```