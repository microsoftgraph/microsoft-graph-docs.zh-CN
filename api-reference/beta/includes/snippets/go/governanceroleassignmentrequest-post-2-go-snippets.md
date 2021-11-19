---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ab8322acaf5ddd671ba3695d2adb5f0d0b1573c
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088120"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewGovernanceRoleAssignmentRequest()
roleDefinitionId := "8b4d1d51-08e9-4254-b0a6-b16177aae376"
requestBody.SetRoleDefinitionId(&roleDefinitionId)
resourceId := "e5e7d29d-5465-45ac-885f-4716a5ee74b5"
requestBody.SetResourceId(&resourceId)
subjectId := "918e54be-12c4-4f4c-a6d3-2ee0e3661c51"
requestBody.SetSubjectId(&subjectId)
assignmentState := "Active"
requestBody.SetAssignmentState(&assignmentState)
type := "UserAdd"
requestBody.SetType(&type)
reason := "Activate the owner role"
requestBody.SetReason(&reason)
schedule := msgraphsdk.NewGovernanceSchedule()
requestBody.SetSchedule(schedule)
type := "Once"
schedule.SetType(&type)
startDateTime, err := time.Parse(time.RFC3339, "2018-05-12T23:28:43.537Z")
schedule.SetStartDateTime(&startDateTime)
duration := "PT9H"
schedule.SetDuration(&duration)
linkedEligibleRoleAssignmentId := "e327f4be-42a0-47a2-8579-0a39b025b394"
requestBody.SetLinkedEligibleRoleAssignmentId(&linkedEligibleRoleAssignmentId)
options := &msgraphsdk.RoleAssignmentRequestsRequestBuilderPostOptions{
    Body: requestBody,
}
privilegedAccessId := "privilegedAccess-id"
result, err := graphClient.PrivilegedAccessById(&privilegedAccessId).RoleAssignmentRequests().Post(options)


```