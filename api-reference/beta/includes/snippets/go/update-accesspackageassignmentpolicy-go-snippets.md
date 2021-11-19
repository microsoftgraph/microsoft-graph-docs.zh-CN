---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6dab067290ef2fdb5c83ad696087c35b2d7b1266
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61084006"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "id": "b2eba9a1-b357-42ee-83a8-336522ed6cbf",
    "accessPackageId": "4c02f928-7752-49aa-8fc8-e286d973a965",
    "displayName": "All Users",
    "description": "All users can request for access to the directory.",
    "canExtend": false,
    "durationInDays": ,
    "expirationDateTime": nil,
    "questions":  []Object {
    }
}
options := &msgraphsdk.AccessPackageAssignmentPolicyRequestBuilderPutOptions{
    Body: requestBody,
}
accessPackageAssignmentPolicyId := "accessPackageAssignmentPolicy-id"
graphClient.IdentityGovernance().EntitlementManagement().AccessPackageAssignmentPoliciesById(&accessPackageAssignmentPolicyId).Put(options)


```