---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d8a5c6e26d668be28b638bde16be6e110069129
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61099174"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEducationAssignment()
displayName := "Reading and review test 09.03 #5"
requestBody.SetDisplayName(&displayName)
instructions := msgraphsdk.NewEducationItemBody()
requestBody.SetInstructions(instructions)
contentType := "text"
instructions.SetContentType(&contentType)
content := "Read chapter 5 and write your review"
instructions.SetContent(&content)
dueDateTime, err := time.Parse(time.RFC3339, "2021-09-10T00:00:00Z")
requestBody.SetDueDateTime(&dueDateTime)
addedStudentAction := "none"
requestBody.SetAddedStudentAction(&addedStudentAction)
options := &msgraphsdk.EducationAssignmentRequestBuilderPatchOptions{
    Body: requestBody,
}
educationClassId := "educationClass-id"
educationAssignmentId := "educationAssignment-id"
graphClient.Education().ClassesById(&educationClassId).AssignmentsById(&educationAssignmentId).Patch(options)


```