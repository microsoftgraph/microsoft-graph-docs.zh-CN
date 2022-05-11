---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0659f4ba451a165f48b737c58abc7b0f9da09d10
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65316365"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPrivilegedRoleAssignmentRequest()
duration := "2"
requestBody.SetDuration(&duration)
reason := "Activate the role for business purpose"
requestBody.SetReason(&reason)
ticketNumber := "234"
requestBody.SetTicketNumber(&ticketNumber)
ticketSystem := "system"
requestBody.SetTicketSystem(&ticketSystem)
schedule := msgraphsdk.NewGovernanceSchedule()
requestBody.SetSchedule(schedule)
startDateTime, err := time.Parse(time.RFC3339, "2018-02-08T02:35:17.903Z")
schedule.SetStartDateTime(&startDateTime)
type := "UserAdd"
requestBody.SetType(&type)
assignmentState := "Active"
requestBody.SetAssignmentState(&assignmentState)
roleId := "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
requestBody.SetRoleId(&roleId)
result, err := graphClient.PrivilegedRoleAssignmentRequests().Post(requestBody)


```