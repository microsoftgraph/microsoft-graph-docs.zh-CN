---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1d1732a753d076cd8369c9e7914e7152814d6722
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61030526"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewClaimsMappingPolicy()
displayName := "UpdateClaimsPolicy"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.ClaimsMappingPolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
claimsMappingPolicyId := "claimsMappingPolicy-id"
graphClient.Policies().ClaimsMappingPoliciesById(&claimsMappingPolicyId).Patch(options)


```