---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 71268d4e92878c067d966ec6ede00555ecdb3bee
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412705"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUnifiedRoleAssignmentMultiple()
requestBody.SetPrincipalIds( []String {
    "0aeec2c1-fee7-4e02-b534-6f920d25b300",
    "2d5386a7-732f-44db-9cf8-f82dd2a1c0e0",
}
options := &msgraphsdk.UnifiedRoleAssignmentMultipleRequestBuilderPatchOptions{
    Body: requestBody,
}
unifiedRoleAssignmentMultipleId := "unifiedRoleAssignmentMultiple-id"
result, err := graphClient.RoleManagement().DeviceManagement().RoleAssignmentsById(&unifiedRoleAssignmentMultipleId).Patch(options)


```