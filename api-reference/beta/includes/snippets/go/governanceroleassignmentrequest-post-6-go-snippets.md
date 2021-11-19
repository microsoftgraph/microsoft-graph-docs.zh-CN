---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ab4dd8e7a696ca0dd2d5454083a126d97d203180
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088934"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewGovernanceRoleAssignmentRequest()
roleDefinitionId := "0e88fd18-50f5-4ee1-9104-01c3ed910065"
requestBody.SetRoleDefinitionId(&roleDefinitionId)
resourceId := "e5e7d29d-5465-45ac-885f-4716a5ee74b5"
requestBody.SetResourceId(&resourceId)
subjectId := "74765671-9ca4-40d7-9e36-2f4a570608a6"
requestBody.SetSubjectId(&subjectId)
assignmentState := "Eligible"
requestBody.SetAssignmentState(&assignmentState)
type := "AdminExtend"
requestBody.SetType(&type)
reason := "extend role assignment"
requestBody.SetReason(&reason)
schedule := msgraphsdk.NewGovernanceSchedule()
requestBody.SetSchedule(schedule)
type := "Once"
schedule.SetType(&type)
startDateTime, err := time.Parse(time.RFC3339, "2018-05-12T23:53:55.327Z")
schedule.SetStartDateTime(&startDateTime)
endDateTime, err := time.Parse(time.RFC3339, "2018-08-10T23:53:55.327Z")
schedule.SetEndDateTime(&endDateTime)
options := &msgraphsdk.RoleAssignmentRequestsRequestBuilderPostOptions{
    Body: requestBody,
}
privilegedAccessId := "privilegedAccess-id"
result, err := graphClient.PrivilegedAccessById(&privilegedAccessId).RoleAssignmentRequests().Post(options)


```