---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e7e1b71a8f08651fb9cd5a610eee9cc6ad47665f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61007295"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewUnifiedRoleAssignment()
principalId := "679a9213-c497-48a4-830a-8d3d25d94ddc"
requestBody.SetPrincipalId(&principalId)
roleDefinitionId := "ae79f266-94d4-4dab-b730-feca7e132178"
requestBody.SetRoleDefinitionId(&roleDefinitionId)
appScopeId := "/AccessPackageCatalog/beedadfe-01d5-4025-910b-84abb9369997"
requestBody.SetAppScopeId(&appScopeId)
options := &msgraphsdk.RoleAssignmentsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.RoleManagement().EntitlementManagement().RoleAssignments().Post(options)


```