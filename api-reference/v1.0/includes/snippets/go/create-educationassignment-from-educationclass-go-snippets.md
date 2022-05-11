---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 51733df6c1a10ad3574c5134ceefa07206d5ce18
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327591"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEducationAssignment()
dueDateTime, err := time.Parse(time.RFC3339, "2021-09-07T00:00:00Z")
requestBody.SetDueDateTime(&dueDateTime)
displayName := "Reading test 09.03 #4"
requestBody.SetDisplayName(&displayName)
instructions := msgraphsdk.NewEducationItemBody()
requestBody.SetInstructions(instructions)
contentType := "text"
instructions.SetContentType(&contentType)
content := "Read chapter 4"
instructions.SetContent(&content)
grading := msgraphsdk.NewEducationAssignmentGradeType()
requestBody.SetGrading(grading)
grading.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.educationAssignmentPointsGradeType",
    "maxPoints": ,
}
assignTo := msgraphsdk.NewEducationAssignmentRecipient()
requestBody.SetAssignTo(assignTo)
assignTo.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.educationAssignmentClassRecipient",
}
status := "draft"
requestBody.SetStatus(&status)
allowStudentsToAddResourcesToSubmission := true
requestBody.SetAllowStudentsToAddResourcesToSubmission(&allowStudentsToAddResourcesToSubmission)
educationClassId := "educationClass-id"
result, err := graphClient.Education().ClassesById(&educationClassId).Assignments().Post(requestBody)


```