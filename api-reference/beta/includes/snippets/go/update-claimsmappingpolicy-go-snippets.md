---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b6a00dc8efeb1c28c884a35f3b175b4fcf1e78e4
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326931"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewClaimsMappingPolicy()
displayName := "UpdateClaimsPolicy"
requestBody.SetDisplayName(&displayName)
claimsMappingPolicyId := "claimsMappingPolicy-id"
graphClient.Policies().ClaimsMappingPoliciesById(&claimsMappingPolicyId).Patch(requestBody)


```