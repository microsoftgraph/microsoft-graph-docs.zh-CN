---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 33b635e334aa5f3dc26fca702c91d84fb75fee23
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328183"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPermissionGrantConditionSet()
permissionType := "delegated"
requestBody.SetPermissionType(&permissionType)
clientApplicationsFromVerifiedPublisherOnly := true
requestBody.SetClientApplicationsFromVerifiedPublisherOnly(&clientApplicationsFromVerifiedPublisherOnly)
permissionGrantPolicyId := "permissionGrantPolicy-id"
result, err := graphClient.Policies().PermissionGrantPoliciesById(&permissionGrantPolicyId).Includes().Post(requestBody)


```