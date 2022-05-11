---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 57ab86d2e19228a213a3fc986e52bbfbd49fb038
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326845"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEducationSubmissionResource()
resource := msgraphsdk.NewEducationResource()
requestBody.SetResource(resource)
displayName := "Wikipedia"
resource.SetDisplayName(&displayName)
resource.SetAdditionalData(map[string]interface{}{
    "link": "https://en.wikipedia.org/wiki/Main_Page",
    "@odata.type": "#microsoft.graph.educationLinkResource",
}
educationClassId := "educationClass-id"
educationAssignmentId := "educationAssignment-id"
educationSubmissionId := "educationSubmission-id"
result, err := graphClient.Education().ClassesById(&educationClassId).AssignmentsById(&educationAssignmentId).SubmissionsById(&educationSubmissionId).Resources().Post(requestBody)


```