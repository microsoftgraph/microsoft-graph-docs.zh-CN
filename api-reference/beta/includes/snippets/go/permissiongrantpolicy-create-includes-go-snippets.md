---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6eb2141c948b5e4c72280bf455d5cf588d22c589
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092904"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPermissionGrantConditionSet()
permissionType := "delegated"
requestBody.SetPermissionType(&permissionType)
clientApplicationsFromVerifiedPublisherOnly := true
requestBody.SetClientApplicationsFromVerifiedPublisherOnly(&clientApplicationsFromVerifiedPublisherOnly)
options := &msgraphsdk.IncludesRequestBuilderPostOptions{
    Body: requestBody,
}
permissionGrantPolicyId := "permissionGrantPolicy-id"
result, err := graphClient.Policies().PermissionGrantPoliciesById(&permissionGrantPolicyId).Includes().Post(options)


```