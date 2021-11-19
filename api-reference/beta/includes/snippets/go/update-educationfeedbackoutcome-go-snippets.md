---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0343f39f2cdf34236815b9e1bd0172fd3a2f0d72
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61099794"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEducationOutcome()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.educationFeedbackOutcome",
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