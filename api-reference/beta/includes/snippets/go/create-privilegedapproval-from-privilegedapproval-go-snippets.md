---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 590b3ffc08209bc9ffa0d03d6220eb73831131cf
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61021508"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewPrivilegedApproval()
userId := "userId-value"
requestBody.SetUserId(&userId)
roleId := "roleId-value"
requestBody.SetRoleId(&roleId)
approvalType := "approvalType-value"
requestBody.SetApprovalType(&approvalType)
approvalState := "approvalState-value"
requestBody.SetApprovalState(&approvalState)
approvalDuration := "datetime-value"
requestBody.SetApprovalDuration(&approvalDuration)
options := &msgraphsdk.PrivilegedApprovalRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.PrivilegedApproval().Post(options)


```