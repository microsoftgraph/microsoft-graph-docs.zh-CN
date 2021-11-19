---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 904854c7c5365b3de7ffeb52d6dd3f60e64a13f2
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61084374"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUnifiedRoleAssignmentScheduleRequest()
action := "AdminAssign"
requestBody.SetAction(&action)
justification := "Assign User Admin to IT Helpdesk (User) group"
requestBody.SetJustification(&justification)
roleDefinitionId := "fdd7a751-b60b-444a-984c-02652fe8fa1c"
requestBody.SetRoleDefinitionId(&roleDefinitionId)
directoryScopeId := "/"
requestBody.SetDirectoryScopeId(&directoryScopeId)
principalId := "07706ff1-46c7-4847-ae33-3003830675a1"
requestBody.SetPrincipalId(&principalId)
scheduleInfo := msgraphsdk.NewRequestSchedule()
requestBody.SetScheduleInfo(scheduleInfo)
startDateTime, err := time.Parse(time.RFC3339, "2021-07-01T00:00:00Z")
scheduleInfo.SetStartDateTime(&startDateTime)
expiration := msgraphsdk.NewExpirationPattern()
scheduleInfo.SetExpiration(expiration)
type := "NoExpiration"
expiration.SetType(&type)
options := &msgraphsdk.RoleAssignmentScheduleRequestsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.RoleManagement().Directory().RoleAssignmentScheduleRequests().Post(options)


```