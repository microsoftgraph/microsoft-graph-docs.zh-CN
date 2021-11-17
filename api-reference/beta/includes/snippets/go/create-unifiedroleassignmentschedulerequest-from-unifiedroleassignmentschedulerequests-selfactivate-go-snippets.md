---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fd64cd6e5c9c58b910772c58408b075c4a44eae4
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61031542"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewUnifiedRoleAssignmentScheduleRequest()
action := "SelfActivate"
requestBody.SetAction(&action)
principalId := "c6ad1942-4afa-47f8-8d48-afb5d8d69d2f"
requestBody.SetPrincipalId(&principalId)
roleDefinitionId := "9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3"
requestBody.SetRoleDefinitionId(&roleDefinitionId)
directoryScopeId := "/"
requestBody.SetDirectoryScopeId(&directoryScopeId)
justification := "Need to update app roles for selected apps."
requestBody.SetJustification(&justification)
scheduleInfo := msgraphsdk.NewRequestSchedule()
requestBody.SetScheduleInfo(scheduleInfo)
startDateTime, err := time.Parse(time.RFC3339, "2021-08-17T17:40:00.000Z")
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