---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e2393a6b881cff97050774e02175c63c3f951a1a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60992236"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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