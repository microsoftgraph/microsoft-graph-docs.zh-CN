---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: af6f0d407ffdf58cc63cdddf40118eb431a21c21
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60984345"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewPermissionGrantConditionSet()
permissionType := "delegated"
requestBody.SetPermissionType(&permissionType)
resourceApplication := "00000003-0000-0000-c000-000000000000"
requestBody.SetResourceApplication(&resourceApplication)
options := &msgraphsdk.ExcludesRequestBuilderPostOptions{
    Body: requestBody,
}
permissionGrantPolicyId := "permissionGrantPolicy-id"
result, err := graphClient.Policies().PermissionGrantPoliciesById(&permissionGrantPolicyId).Excludes().Post(options)


```