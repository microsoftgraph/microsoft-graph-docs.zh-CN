---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6720fe4d1a7307389c80e0d5a67659334c1d65d1
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412471"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAuthorizationPolicy()
allowedToUseSSPR := true
requestBody.SetAllowedToUseSSPR(&allowedToUseSSPR)
options := &msgraphsdk.AuthorizationPolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
result, err := graphClient.Policies().AuthorizationPolicy().Patch(options)


```