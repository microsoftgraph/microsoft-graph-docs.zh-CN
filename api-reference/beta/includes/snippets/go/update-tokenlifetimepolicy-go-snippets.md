---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a8441b4c52a9878bef60785ff618690df326d0c1
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089817"
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
graphClient.Policies().TokenLifetimePoliciesById(&tokenLifetimePolicyId).Patch(options)


```