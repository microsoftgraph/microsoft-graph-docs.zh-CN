---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc3c8dc4a2e58b6ea943898cf5059bd3c5169ba9
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328101"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEducationSubmissionResource()
resource := msgraphsdk.NewEducationResource()
requestBody.SetResource(resource)
displayName := "_FTP_EDC-61424749-250820211136.pdf"
resource.SetDisplayName(&displayName)
resource.SetAdditionalData(map[string]interface{}{
    "fileUrl": "https://graph.microsoft.com/beta/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXodJYOAkI7rTLhw7ME_e42J/items/01QTY63RL45XVPGDBRW5FLDR62Z5TCMGG3",
    "@odata.type": "#microsoft.graph.educationFileResource",
}
educationClassId := "educationClass-id"
educationAssignmentId := "educationAssignment-id"
educationSubmissionId := "educationSubmission-id"
result, err := graphClient.Education().ClassesById(&educationClassId).AssignmentsById(&educationAssignmentId).SubmissionsById(&educationSubmissionId).Resources().Post(requestBody)


```