---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fe90bea3c008cda3e7041774a20823ada428139d
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61087567"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAccessPackageAssignmentRequest()
requestType := "AdminAdd"
requestBody.SetRequestType(&requestType)
accessPackageAssignment := msgraphsdk.NewAccessPackageAssignment()
requestBody.SetAccessPackageAssignment(accessPackageAssignment)
accessPackageAssignment.SetAdditionalData(map[string]interface{}{
    "assignmentPolicyId": "2264bf65-76ba-417b-a27d-54d291f0cbc8",
    "accessPackageId": "a914b616-e04e-476b-aa37-91038f0b165b",
}
options := &msgraphsdk.AccessPackageAssignmentRequestsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageAssignmentRequests().Post(options)


```