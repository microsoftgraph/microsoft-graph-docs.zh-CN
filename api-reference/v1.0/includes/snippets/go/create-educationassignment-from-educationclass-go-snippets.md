---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2f81d6108e00b02e65c1cedd7fe6da5d87d53b2f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61024694"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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
options := &msgraphsdk.AssignmentsRequestBuilderPostOptions{
    Body: requestBody,
}
educationClassId := "educationClass-id"
result, err := graphClient.Education().ClassesById(&educationClassId).Assignments().Post(options)


```