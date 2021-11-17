---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b9e49837fbdb70e390c676fa53c02df5daaa9c11
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60984324"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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