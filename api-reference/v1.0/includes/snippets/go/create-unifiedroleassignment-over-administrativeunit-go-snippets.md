---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b20f250d11268af40e1a54facbeecf6737b68d5
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61006120"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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
options := &msgraphsdk.RoleAssignmentsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.RoleManagement().Directory().RoleAssignments().Post(options)


```