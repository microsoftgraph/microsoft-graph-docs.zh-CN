---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e99c47b8387bb51398525370d8278a753a06915c
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60995643"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewAppManagementPolicy()
isEnabled := false
requestBody.SetIsEnabled(&isEnabled)
options := &msgraphsdk.AppManagementPolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
appManagementPolicyId := "appManagementPolicy-id"
graphClient.Policies().AppManagementPoliciesById(&appManagementPolicyId).Patch(options)


```