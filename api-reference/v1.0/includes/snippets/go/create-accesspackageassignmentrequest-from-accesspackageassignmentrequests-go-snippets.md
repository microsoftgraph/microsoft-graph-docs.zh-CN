---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ce8a592e50209b20fb8f57d5b10b29cf5c37740
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62117550"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAccessPackageAssignmentRequest()
requestType := "AdminRemove"
requestBody.SetRequestType(&requestType)
assignment := msgraphsdk.NewAccessPackageAssignment()
requestBody.SetAssignment(assignment)
id := "a6bb6942-3ae1-4259-9908-0133aaee9377"
assignment.SetId(&id)
options := &msgraphsdk.AssignmentRequestsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.IdentityGovernance().EntitlementManagement().AssignmentRequests().Post(options)


```