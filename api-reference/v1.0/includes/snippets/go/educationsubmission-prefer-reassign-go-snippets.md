---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f2bfc73bb31f1f4d73e40fc879ef8ffeaefda36a
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325905"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

headers := map[string]string{
    "Prefer": "include-unknown-enum-members"
}
options := &msgraphsdk.ReassignRequestBuilderPostRequestConfiguration{
    Headers: headers,
}
educationClassId := "educationClass-id"
educationAssignmentId := "educationAssignment-id"
educationSubmissionId := "educationSubmission-id"
result, err := graphClient.Education().ClassesById(&educationClassId).AssignmentsById(&educationAssignmentId).SubmissionsById(&educationSubmissionId).Reassign(educationClass-id, educationAssignment-id, educationSubmission-id).PostWithRequestConfigurationAndResponseHandler(options, nil)


```