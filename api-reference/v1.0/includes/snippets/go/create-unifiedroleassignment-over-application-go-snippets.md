---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 23fe3f0e7cd1a97754cb77d3d8e6d77b2b6969dc
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092972"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUnifiedRoleAssignment()
principalId := "6b937a9d-c731-465b-a844-2d5b5368c161"
requestBody.SetPrincipalId(&principalId)
roleDefinitionId := "9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3"
requestBody.SetRoleDefinitionId(&roleDefinitionId)
directoryScopeId := "/661e1310-bd76-4795-89a7-8f3c8f855bfc"
requestBody.SetDirectoryScopeId(&directoryScopeId)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
}
options := &msgraphsdk.RoleAssignmentsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.RoleManagement().Directory().RoleAssignments().Post(options)


```