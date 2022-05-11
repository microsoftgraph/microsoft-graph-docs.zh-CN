---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3902eddaf2523da1072e65a6c43e297063faa44d
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328925"
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
result, err := graphClient.RoleManagement().EntitlementManagement().RoleAssignments().Post(requestBody)


```