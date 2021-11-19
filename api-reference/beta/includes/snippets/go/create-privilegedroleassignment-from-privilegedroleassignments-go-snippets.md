---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2f449b8bd02f507eece5e3f30a582020c8e00a1b
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61096895"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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