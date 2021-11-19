---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 30720bfd11d0666ceb26450cc52848ef31e312e5
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097679"
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
graphClient.IdentityGovernance().EntitlementManagement().Settings().Patch(options)


```