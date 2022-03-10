---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f9fd5dd6b6aff8405518612e4b2987165f502fd3
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412467"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAuthorizationPolicy()
blockMsolPowerShell := true
requestBody.SetBlockMsolPowerShell(&blockMsolPowerShell)
options := &msgraphsdk.AuthorizationPolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
result, err := graphClient.Policies().AuthorizationPolicy().Patch(options)


```