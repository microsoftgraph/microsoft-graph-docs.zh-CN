---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3509d799352d998e3c0deaf902016660ff9c1cb
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61021362"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewIdentitySecurityDefaultsEnforcementPolicy()
isEnabled := false
requestBody.SetIsEnabled(&isEnabled)
options := &msgraphsdk.IdentitySecurityDefaultsEnforcementPolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
graphClient.Policies().IdentitySecurityDefaultsEnforcementPolicy().Patch(options)


```