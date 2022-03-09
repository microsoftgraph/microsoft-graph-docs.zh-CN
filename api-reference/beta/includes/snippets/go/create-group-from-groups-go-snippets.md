---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 449d5e9bae0ea2744a34eb5233e3d7aaa135932d
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63394374"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/odata/groups('dc3d2ce5-7c5e-4dca-a0ef-2145bf6e53ef')",
}
options := &msgraphsdk.GroupRequestBuilderPostOptions{
    Body: requestBody,
}
mobilityManagementPolicyId := "mobilityManagementPolicy-id"
groupId := "group-id"
graphClient.Policies().MobileDeviceManagementPoliciesById(&mobilityManagementPolicyId).IncludedGroupsById(&groupId).Post(options)


```