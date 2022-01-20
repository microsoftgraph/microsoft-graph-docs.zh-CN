---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c5c6658bc8733f24e1e4f96451e1d052b3f88032
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62129846"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAccessPackageAssignmentRequest()
requestType := "UserAdd"
requestBody.SetRequestType(&requestType)
accessPackageAssignment := msgraphsdk.NewAccessPackageAssignment()
requestBody.SetAccessPackageAssignment(accessPackageAssignment)
targetId := "46184453-e63b-4f20-86c2-c557ed5d5df9"
accessPackageAssignment.SetTargetId(&targetId)
assignmentPolicyId := "2264bf65-76ba-417b-a27d-54d291f0cbc8"
accessPackageAssignment.SetAssignmentPolicyId(&assignmentPolicyId)
accessPackageId := "a914b616-e04e-476b-aa37-91038f0b165b"
accessPackageAssignment.SetAccessPackageId(&accessPackageId)
requestBody.SetAnswers( []AccessPackageAnswer {
    msgraphsdk.NewAccessPackageAnswer(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.accessPackageAnswerString",
        "value": "Arizona",
    }
    msgraphsdk.NewAccessPackageAnswer(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.accessPackageAnswerString",
        "value": "Need access to marketing campaign material",
    }
}
options := &msgraphsdk.AccessPackageAssignmentRequestsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageAssignmentRequests().Post(options)


```