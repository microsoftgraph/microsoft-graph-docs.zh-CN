---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 00b1711e8a3597fc956d500d7ec60ba2d2800bcc
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61096725"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAccessPackageAssignmentRequest()
requestType := "UserAdd"
requestBody.SetRequestType(&requestType)
accessPackageAssignment := msgraphsdk.NewAccessPackageAssignment()
requestBody.SetAccessPackageAssignment(accessPackageAssignment)
accessPackageAssignment.SetAdditionalData(map[string]interface{}{
    "targetId": "46184453-e63b-4f20-86c2-c557ed5d5df9",
    "assignmentPolicyId": "2264bf65-76ba-417b-a27d-54d291f0cbc8",
    "accessPackageId": "a914b616-e04e-476b-aa37-91038f0b165b",
}
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