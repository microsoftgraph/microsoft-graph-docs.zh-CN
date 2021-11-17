---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b343b3dd483669e0f2994a2f514d1c5251c14e9e
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61017190"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewUnifiedRoleAssignmentMultiple()
displayName := "NewName"
requestBody.SetDisplayName(&displayName)
description := "A new roleAssignment"
requestBody.SetDescription(&description)
options := &msgraphsdk.UnifiedRoleAssignmentMultipleRequestBuilderPatchOptions{
    Body: requestBody,
}
unifiedRoleAssignmentMultipleId := "unifiedRoleAssignmentMultiple-id"
graphClient.RoleManagement().CloudPC().RoleAssignmentsById(&unifiedRoleAssignmentMultipleId).Patch(options)


```