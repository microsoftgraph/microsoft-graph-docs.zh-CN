---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 13c261ccb75e43da11d14a6acf7fa7e4b6129d58
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65946808"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/odata/groups('dc3d2ce5-7c5e-4dca-a0ef-2145bf6e53ef')",
}
mobilityManagementPolicyId := "mobilityManagementPolicy-id"
result, err := graphClient.Policies().MobileDeviceManagementPoliciesById(&mobilityManagementPolicyId).IncludedGroups().$ref().Post(requestBody)


```