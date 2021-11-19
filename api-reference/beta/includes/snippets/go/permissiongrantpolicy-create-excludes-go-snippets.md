---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: abc3412d097f7a64f34632615903480fb0dad57b
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61099207"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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