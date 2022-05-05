---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a9cc5784a42d52a5232aaa9398b6be0cbe03df86
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65206982"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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