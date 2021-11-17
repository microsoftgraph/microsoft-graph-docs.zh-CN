---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8631fcb41f12bac57f7b123f4fa1d28bfddc4a84
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61024848"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewEntitlementManagementSettings()
externalUserLifecycleAction := "None"
requestBody.SetExternalUserLifecycleAction(&externalUserLifecycleAction)
options := &msgraphsdk.SettingsRequestBuilderPatchOptions{
    Body: requestBody,
}
graphClient.IdentityGovernance().EntitlementManagement().Settings().Patch(options)


```