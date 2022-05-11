---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7cd127fd8e139866988fbc6c9a5473f70efbc1f3
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326498"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUnifiedRoleAssignment()
roleDefinitionId := "fe930be7-5e62-47db-91af-98c3a49a38b1"
requestBody.SetRoleDefinitionId(&roleDefinitionId)
principalId := "f8ca5a85-489a-49a0-b555-0a6d81e56f0d"
requestBody.SetPrincipalId(&principalId)
directoryScopeId := "/administrativeUnits/5d107bba-d8e2-4e13-b6ae-884be90e5d1a"
requestBody.SetDirectoryScopeId(&directoryScopeId)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
}
result, err := graphClient.RoleManagement().Directory().RoleAssignments().Post(requestBody)


```