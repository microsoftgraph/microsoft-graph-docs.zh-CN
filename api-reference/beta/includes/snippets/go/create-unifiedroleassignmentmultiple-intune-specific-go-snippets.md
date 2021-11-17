---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3414ea37bfa5bd5004b9046d9f632f8a466bc5d8
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60980013"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewUnifiedRoleAssignmentMultiple()
displayName := "My test role assignment 1"
requestBody.SetDisplayName(&displayName)
roleDefinitionId := "c2cf284d-6c41-4e6b-afac-4b80928c9034"
requestBody.SetRoleDefinitionId(&roleDefinitionId)
requestBody.SetPrincipalIds( []String {
    "f8ca5a85-489a-49a0-b555-0a6d81e56f0d",
    "c1518aa9-4da5-4c84-a902-a31404023890",
}
requestBody.SetAppScopeIds( []String {
    "allDevices",
}
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
}
options := &msgraphsdk.RoleAssignmentsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.RoleManagement().DeviceManagement().RoleAssignments().Post(options)


```