---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 819bca3ed16588aadd2bb7465678e881c45bc9a1
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092901"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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