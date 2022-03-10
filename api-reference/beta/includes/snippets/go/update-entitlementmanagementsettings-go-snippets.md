---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4d5d0b1d2d283be02f12b68886d4546d8b8b1f1b
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412041"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEntitlementManagementSettings()
externalUserLifecycleAction := "None"
requestBody.SetExternalUserLifecycleAction(&externalUserLifecycleAction)
options := &msgraphsdk.SettingsRequestBuilderPatchOptions{
    Body: requestBody,
}
result, err := graphClient.IdentityGovernance().EntitlementManagement().Settings().Patch(options)


```