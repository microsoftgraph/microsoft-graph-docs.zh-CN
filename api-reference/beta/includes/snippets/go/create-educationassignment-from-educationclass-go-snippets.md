---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ddad086adfe4a36822a350a53c7a751241a7648
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61083960"
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
options := &msgraphsdk.AssignmentsRequestBuilderPostOptions{
    Body: requestBody,
}
educationClassId := "educationClass-id"
result, err := graphClient.Education().ClassesById(&educationClassId).Assignments().Post(options)


```