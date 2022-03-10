---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3243653f62c3f5ff20e3181f270a7c5e23bd3d9d
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412704"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUnifiedRoleAssignmentMultiple()
displayName := "NewName"
requestBody.SetDisplayName(&displayName)
description := "A new roleAssignment"
requestBody.SetDescription(&description)
options := &msgraphsdk.UnifiedRoleAssignmentMultipleRequestBuilderPatchOptions{
    Body: requestBody,
}
unifiedRoleAssignmentMultipleId := "unifiedRoleAssignmentMultiple-id"
result, err := graphClient.RoleManagement().CloudPC().RoleAssignmentsById(&unifiedRoleAssignmentMultipleId).Patch(options)


```