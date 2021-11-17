---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ff50d6e981df410c63a2e85c33c7db57c6e859e3
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61017192"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewUnifiedRoleAssignmentMultiple()
requestBody.SetPrincipalIds( []String {
    "0aeec2c1-fee7-4e02-b534-6f920d25b300",
    "2d5386a7-732f-44db-9cf8-f82dd2a1c0e0",
}
options := &msgraphsdk.UnifiedRoleAssignmentMultipleRequestBuilderPatchOptions{
    Body: requestBody,
}
unifiedRoleAssignmentMultipleId := "unifiedRoleAssignmentMultiple-id"
graphClient.RoleManagement().DeviceManagement().RoleAssignmentsById(&unifiedRoleAssignmentMultipleId).Patch(options)


```