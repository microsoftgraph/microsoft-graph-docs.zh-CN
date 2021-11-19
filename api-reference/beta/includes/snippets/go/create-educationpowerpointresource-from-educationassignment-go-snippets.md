---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 388b8a385bf351b498e4065e6b4126cec21649b0
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089343"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEducationAssignmentResource()
distributeForStudentWork := false
requestBody.SetDistributeForStudentWork(&distributeForStudentWork)
resource := msgraphsdk.NewEducationResource()
requestBody.SetResource(resource)
displayName := "state diagram.pptx"
resource.SetDisplayName(&displayName)
resource.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.educationPowerPointResource",
    "fileUrl": "https://graph.microsoft.com/beta/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXoOOmEQNO79QpIMPdOmY3nf/items/01QTY63RN327OXRN6EVFE2Q5FRJZTN5EOJ",
}
options := &msgraphsdk.ResourcesRequestBuilderPostOptions{
    Body: requestBody,
}
educationClassId := "educationClass-id"
educationAssignmentId := "educationAssignment-id"
result, err := graphClient.Education().ClassesById(&educationClassId).AssignmentsById(&educationAssignmentId).Resources().Post(options)


```