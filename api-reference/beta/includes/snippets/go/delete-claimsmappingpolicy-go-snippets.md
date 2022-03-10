---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1dda69a0e2bd6946036b3868cc2d05a0a854723c
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411916"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

claimsMappingPolicyId := "claimsMappingPolicy-id"
result, err := graphClient.Policies().ClaimsMappingPoliciesById(&claimsMappingPolicyId).Delete(nil)


```