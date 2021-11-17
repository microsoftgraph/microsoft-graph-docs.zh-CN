---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 43f1ae34ce7fcf4e637ba91acd6b52f622ddc617
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61016324"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewEducationSubmissionResource()
resource := msgraphsdk.NewEducationResource()
requestBody.SetResource(resource)
displayName := "_FTP_EDC-61424749-250820211136.pdf"
resource.SetDisplayName(&displayName)
resource.SetAdditionalData(map[string]interface{}{
    "fileUrl": "https://graph.microsoft.com/v1.0/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXodJYOAkI7rTLhw7ME_e42J/items/01QTY63RL45XVPGDBRW5FLDR62Z5TCMGG3",
    "@odata.type": "#microsoft.graph.educationFileResource",
}
options := &msgraphsdk.ResourcesRequestBuilderPostOptions{
    Body: requestBody,
}
educationClassId := "educationClass-id"
educationAssignmentId := "educationAssignment-id"
educationSubmissionId := "educationSubmission-id"
result, err := graphClient.Education().ClassesById(&educationClassId).AssignmentsById(&educationAssignmentId).SubmissionsById(&educationSubmissionId).Resources().Post(options)


```