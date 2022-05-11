---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fdcd89cc9dfb41009a63a06cadeb60a51f28fd73
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326851"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEducationSubmissionResource()
resource := msgraphsdk.NewEducationResource()
requestBody.SetResource(resource)
displayName := "category.jpg"
resource.SetDisplayName(&displayName)
resource.SetAdditionalData(map[string]interface{}{
    "fileUrl": "https://graph.microsoft.com/v1.0/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXodJYOAkI7rTLhw7ME_e42J/items/01QTY63RK2WLKUUBAA4ZBKXNBL6QFC2TKG",
    "@odata.type": "#microsoft.graph.educationMediaResource",
}
educationClassId := "educationClass-id"
educationAssignmentId := "educationAssignment-id"
educationSubmissionId := "educationSubmission-id"
result, err := graphClient.Education().ClassesById(&educationClassId).AssignmentsById(&educationAssignmentId).SubmissionsById(&educationSubmissionId).Resources().Post(requestBody)


```