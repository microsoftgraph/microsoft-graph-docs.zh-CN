---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 921dc27842fd51ea383b37e88421b931c47f1138
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60980346"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
reason := "reason-value"
requestBody.SetReason(&reason)
duration := "duration-value"
requestBody.SetDuration(&duration)
ticketNumber := "ticketNumber-value"
requestBody.SetTicketNumber(&ticketNumber)
ticketSystem := "ticketSystem-value"
requestBody.SetTicketSystem(&ticketSystem)
options := &msgraphsdk.SelfActivateRequestBuilderPostOptions{
    Body: requestBody,
}
privilegedRoleId := "privilegedRole-id"
result, err := graphClient.PrivilegedRolesById(&privilegedRoleId).SelfActivate().Post(options)


```