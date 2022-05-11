---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 65365fed4cbbfa59ba75d5adbab7c63c103d1f38
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328127"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUnifiedRoleAssignmentMultiple()
requestBody.SetPrincipalIds( []String {
    "0aeec2c1-fee7-4e02-b534-6f920d25b300",
    "2d5386a7-732f-44db-9cf8-f82dd2a1c0e0",
}
unifiedRoleAssignmentMultipleId := "unifiedRoleAssignmentMultiple-id"
graphClient.RoleManagement().DeviceManagement().RoleAssignmentsById(&unifiedRoleAssignmentMultipleId).Patch(requestBody)


```