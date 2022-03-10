---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f0bc22b710044ea718738387347cee84b4200c9b
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412600"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewIdentitySecurityDefaultsEnforcementPolicy()
isEnabled := false
requestBody.SetIsEnabled(&isEnabled)
options := &msgraphsdk.IdentitySecurityDefaultsEnforcementPolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
result, err := graphClient.Policies().IdentitySecurityDefaultsEnforcementPolicy().Patch(options)


```