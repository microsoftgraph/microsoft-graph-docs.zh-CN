---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6326a329d0229d0fce61fa815a3ed40702b09547
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60985710"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewPermissionGrantPolicy()
id := "my-custom-consent-policy"
requestBody.SetId(&id)
displayName := "Custom application consent policy"
requestBody.SetDisplayName(&displayName)
description := "A custom permission grant policy to customize conditions for granting consent."
requestBody.SetDescription(&description)
options := &msgraphsdk.PermissionGrantPoliciesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Policies().PermissionGrantPolicies().Post(options)


```