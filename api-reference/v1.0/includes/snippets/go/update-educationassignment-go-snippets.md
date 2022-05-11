---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ea911b22bba5b8f431de2d914e155a60dc9edbd
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326344"
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
educationClassId := "educationClass-id"
educationAssignmentId := "educationAssignment-id"
graphClient.Education().ClassesById(&educationClassId).AssignmentsById(&educationAssignmentId).Patch(requestBody)


```