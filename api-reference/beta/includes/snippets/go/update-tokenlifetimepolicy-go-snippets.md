---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 96fc0ec8e291e5d7cd60d9ee219e5f3e8ee82916
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412144"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTokenLifetimePolicy()
requestBody.SetDefinition( []String {
    "definition-value",
}
displayName := "displayName-value"
requestBody.SetDisplayName(&displayName)
isOrganizationDefault := true
requestBody.SetIsOrganizationDefault(&isOrganizationDefault)
options := &msgraphsdk.TokenLifetimePolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
tokenLifetimePolicyId := "tokenLifetimePolicy-id"
result, err := graphClient.Policies().TokenLifetimePoliciesById(&tokenLifetimePolicyId).Patch(options)


```