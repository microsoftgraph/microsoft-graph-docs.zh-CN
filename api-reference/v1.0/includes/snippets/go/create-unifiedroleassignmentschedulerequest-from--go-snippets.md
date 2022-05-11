---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 99140c7ecf781bda0d34031cc90f9413c54e163a
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328524"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUnifiedRoleAssignmentScheduleRequest()
action := "adminAssign"
requestBody.SetAction(&action)
justification := "Assign Groups Admin to IT Helpdesk group"
requestBody.SetJustification(&justification)
roleDefinitionId := "fdd7a751-b60b-444a-984c-02652fe8fa1c"
requestBody.SetRoleDefinitionId(&roleDefinitionId)
directoryScopeId := "/"
requestBody.SetDirectoryScopeId(&directoryScopeId)
principalId := "071cc716-8147-4397-a5ba-b2105951cc0b"
requestBody.SetPrincipalId(&principalId)
scheduleInfo := msgraphsdk.NewRequestSchedule()
requestBody.SetScheduleInfo(scheduleInfo)
startDateTime, err := time.Parse(time.RFC3339, "2022-04-10T00:00:00Z")
scheduleInfo.SetStartDateTime(&startDateTime)
expiration := msgraphsdk.NewExpirationPattern()
scheduleInfo.SetExpiration(expiration)
type := "NoExpiration"
expiration.SetType(&type)
result, err := graphClient.RoleManagement().Directory().RoleAssignmentScheduleRequests().Post(requestBody)


```