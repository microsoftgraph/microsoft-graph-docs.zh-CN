---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 17890b2765e16607e665c00e00093e1b1097cb8b
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412078"
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
authorizationPolicyId := "authorizationPolicy-id"
result, err := graphClient.Policies().AuthorizationPolicyById(&authorizationPolicyId).Patch(options)


```