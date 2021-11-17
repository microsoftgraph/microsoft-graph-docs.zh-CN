---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 91caf58b3862e5edccf4887cf900accb64b31704
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60980290"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewPrivilegedRoleAssignment()
userId := "userId-value"
requestBody.SetUserId(&userId)
roleId := "roleId-value"
requestBody.SetRoleId(&roleId)
options := &msgraphsdk.PrivilegedRoleAssignmentsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.PrivilegedRoleAssignments().Post(options)


```