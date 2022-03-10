---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 56a75420c129ccfa348dbf0602657af01087e856
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411726"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/v1.0/policies/tokenLifetimePolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9",
}
options := &msgraphsdk.TokenLifetimePolicyRequestBuilderPostOptions{
    Body: requestBody,
}
applicationId := "application-id"
tokenLifetimePolicyId := "tokenLifetimePolicy-id"
graphClient.ApplicationsById(&applicationId).TokenLifetimePoliciesById(&tokenLifetimePolicyId).Post(options)


```