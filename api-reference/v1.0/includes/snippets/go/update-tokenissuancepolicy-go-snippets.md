---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 66b46fe7977eeb31f633bc481e7c1088795f503f
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61095235"
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
graphClient.Policies().TokenIssuancePoliciesById(&tokenIssuancePolicyId).Patch(options)


```