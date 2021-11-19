---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4c1db55d82a034b0269e51a64ce79ab4ab6c972a
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61102453"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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