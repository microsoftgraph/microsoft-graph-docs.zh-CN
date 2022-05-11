---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c50022bfaac1790d4e506014eaa4d3b363ae43c4
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328726"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewGovernanceRoleAssignmentRequest()
roleDefinitionId := "70521f3e-3b95-4e51-b4d2-a2f485b02103"
requestBody.SetRoleDefinitionId(&roleDefinitionId)
resourceId := "e5e7d29d-5465-45ac-885f-4716a5ee74b5"
requestBody.SetResourceId(&resourceId)
subjectId := "1566d11d-d2b6-444a-a8de-28698682c445"
requestBody.SetSubjectId(&subjectId)
assignmentState := "Eligible"
requestBody.SetAssignmentState(&assignmentState)
type := "AdminUpdate"
requestBody.SetType(&type)
schedule := msgraphsdk.NewGovernanceSchedule()
requestBody.SetSchedule(schedule)
type := "Once"
schedule.SetType(&type)
startDateTime, err := time.Parse(time.RFC3339, "2018-03-08T05:42:45.317Z")
schedule.SetStartDateTime(&startDateTime)
endDateTime, err := time.Parse(time.RFC3339, "2018-06-05T05:42:31.000Z")
schedule.SetEndDateTime(&endDateTime)
privilegedAccessId := "privilegedAccess-id"
result, err := graphClient.PrivilegedAccessById(&privilegedAccessId).RoleAssignmentRequests().Post(requestBody)


```