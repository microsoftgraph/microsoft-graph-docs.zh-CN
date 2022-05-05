---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fe519d87310e97fc8e6ab20752f6ffc5304a28dc
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65206771"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUnifiedRoleAssignmentScheduleRequest()
action := "selfActivate"
requestBody.SetAction(&action)
principalId := "071cc716-8147-4397-a5ba-b2105951cc0b"
requestBody.SetPrincipalId(&principalId)
roleDefinitionId := "8424c6f0-a189-499e-bbd0-26c1753c96d4"
requestBody.SetRoleDefinitionId(&roleDefinitionId)
directoryScopeId := "/"
requestBody.SetDirectoryScopeId(&directoryScopeId)
justification := "I need access to the Attribute Administrator role to manage attributes to be assigned to restricted AUs"
requestBody.SetJustification(&justification)
scheduleInfo := msgraphsdk.NewRequestSchedule()
requestBody.SetScheduleInfo(scheduleInfo)
startDateTime, err := time.Parse(time.RFC3339, "2022-04-14T00:00:00.000Z")
scheduleInfo.SetStartDateTime(&startDateTime)
expiration := msgraphsdk.NewExpirationPattern()
scheduleInfo.SetExpiration(expiration)
type := "AfterDuration"
expiration.SetType(&type)
duration := "PT5H"
expiration.SetDuration(&duration)
ticketInfo := msgraphsdk.NewTicketInfo()
requestBody.SetTicketInfo(ticketInfo)
ticketNumber := "CONTOSO:Normal-67890"
ticketInfo.SetTicketNumber(&ticketNumber)
ticketSystem := "MS Project"
ticketInfo.SetTicketSystem(&ticketSystem)
options := &msgraphsdk.RoleAssignmentScheduleRequestsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.RoleManagement().Directory().RoleAssignmentScheduleRequests().Post(options)


```