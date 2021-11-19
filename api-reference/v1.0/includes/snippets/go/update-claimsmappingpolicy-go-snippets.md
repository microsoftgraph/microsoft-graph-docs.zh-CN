---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 91447346cdf2a428a4f1a7caa48a8044a7ba6240
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090203"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewClaimsMappingPolicy()
displayName := "UpdateClaimsPolicy"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.ClaimsMappingPolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
claimsMappingPolicyId := "claimsMappingPolicy-id"
graphClient.Policies().ClaimsMappingPoliciesById(&claimsMappingPolicyId).Patch(options)


```