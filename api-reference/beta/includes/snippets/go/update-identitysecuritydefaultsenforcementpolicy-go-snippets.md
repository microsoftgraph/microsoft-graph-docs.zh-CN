---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 48f8d346fb7869743106d307c3fa25af7d5a6ef4
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61085380"
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
graphClient.Policies().IdentitySecurityDefaultsEnforcementPolicy().Patch(options)


```