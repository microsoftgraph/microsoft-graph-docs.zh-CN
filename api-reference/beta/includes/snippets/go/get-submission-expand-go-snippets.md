---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f561b971e2eeb263ac761a6a3721efd6d1f0dd01
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328952"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.EducationSubmissionRequestBuilderGetQueryParameters{
    Expand: "*",
}
options := &msgraphsdk.EducationSubmissionRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
educationClassId := "educationClass-id"
educationAssignmentId := "educationAssignment-id"
educationSubmissionId := "educationSubmission-id"
result, err := graphClient.Education().ClassesById(&educationClassId).AssignmentsById(&educationAssignmentId).SubmissionsById(&educationSubmissionId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```