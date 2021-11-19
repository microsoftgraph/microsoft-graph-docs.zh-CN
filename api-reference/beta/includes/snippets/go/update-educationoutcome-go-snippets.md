---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ef554f7a0401b111eb2d80a7bddfb8c3de2b36a
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090070"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEducationOutcome()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.educationRubricOutcome",
    "rubricQualityFeedback":  []Object {
    }
    "rubricQualitySelectedLevels":  []Object {
    }
}
options := &msgraphsdk.EducationOutcomeRequestBuilderPatchOptions{
    Body: requestBody,
}
educationClassId := "educationClass-id"
educationAssignmentId := "educationAssignment-id"
educationSubmissionId := "educationSubmission-id"
educationOutcomeId := "educationOutcome-id"
graphClient.Education().ClassesById(&educationClassId).AssignmentsById(&educationAssignmentId).SubmissionsById(&educationSubmissionId).OutcomesById(&educationOutcomeId).Patch(options)


```