---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eb494edc2db198d8bed904d8901e4546a74cc561
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61095917"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEducationAssignmentResource()
distributeForStudentWork := false
requestBody.SetDistributeForStudentWork(&distributeForStudentWork)
resource := msgraphsdk.NewEducationResource()
requestBody.SetResource(resource)
displayName := "Issues and PR in guthub.docx"
resource.SetDisplayName(&displayName)
resource.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.educationWordResource",
    "fileUrl": "https://graph.microsoft.com/v1.0/drives/b!DPA6q59Tw0mtgmyXRUmrQRqBZTesG-lMkl1cBmvvMeUEWrOk89nKRpUEr4ZhNYBc/items/016XPCQEELISJB7NVNVBAK7V4UIF6Q27U2",
}
options := &msgraphsdk.ResourcesRequestBuilderPostOptions{
    Body: requestBody,
}
educationClassId := "educationClass-id"
educationAssignmentId := "educationAssignment-id"
result, err := graphClient.Education().ClassesById(&educationClassId).AssignmentsById(&educationAssignmentId).Resources().Post(options)


```