---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e7d967988c324f823d4d648ed91214060f782e0f
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328922"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUnifiedRoleAssignmentMultiple()
displayName := "My test role assignment 1"
requestBody.SetDisplayName(&displayName)
description := "My role assignment description"
requestBody.SetDescription(&description)
roleDefinitionId := "b5c08161-a7af-481c-ace2-a20a69a48fb1"
requestBody.SetRoleDefinitionId(&roleDefinitionId)
requestBody.SetPrincipalIds( []String {
    "f8ca5a85-489a-49a0-b555-0a6d81e56f0d",
    "c1518aa9-4da5-4c84-a902-a31404023890",
}
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
}
result, err := graphClient.RoleManagement().CloudPC().RoleAssignments().Post(requestBody)


```