---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9be88fe94ca693a574fad5dfbb4dd1948cdab635
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328921"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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
result, err := graphClient.RoleManagement().DeviceManagement().RoleAssignments().Post(requestBody)


```