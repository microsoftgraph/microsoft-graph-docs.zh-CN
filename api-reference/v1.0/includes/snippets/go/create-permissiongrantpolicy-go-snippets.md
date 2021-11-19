---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 658c7c3a15f684ab1264d1f5bd85321767d405d3
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61099514"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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