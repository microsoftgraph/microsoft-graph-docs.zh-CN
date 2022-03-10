---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 19d4d944d0717a85eb1e1facf0856eee2986564e
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412575"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTokenIssuancePolicy()
requestBody.SetDefinition( []String {
    "definition-value",
}
displayName := "displayName-value"
requestBody.SetDisplayName(&displayName)
isOrganizationDefault := true
requestBody.SetIsOrganizationDefault(&isOrganizationDefault)
options := &msgraphsdk.TokenIssuancePolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
tokenIssuancePolicyId := "tokenIssuancePolicy-id"
result, err := graphClient.Policies().TokenIssuancePoliciesById(&tokenIssuancePolicyId).Patch(options)


```