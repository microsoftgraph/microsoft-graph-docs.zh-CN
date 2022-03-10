---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b98c5bc437d0569a14dadac98a4382feccd78a28
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411847"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAppManagementPolicy()
isEnabled := false
requestBody.SetIsEnabled(&isEnabled)
options := &msgraphsdk.AppManagementPolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
appManagementPolicyId := "appManagementPolicy-id"
result, err := graphClient.Policies().AppManagementPoliciesById(&appManagementPolicyId).Patch(options)


```