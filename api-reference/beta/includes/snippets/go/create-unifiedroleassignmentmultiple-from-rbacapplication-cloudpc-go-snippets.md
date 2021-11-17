---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6cb2bfced3d735df090b338c3c2452ae560e5c29
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60980015"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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
options := &msgraphsdk.RoleAssignmentsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.RoleManagement().CloudPC().RoleAssignments().Post(options)


```