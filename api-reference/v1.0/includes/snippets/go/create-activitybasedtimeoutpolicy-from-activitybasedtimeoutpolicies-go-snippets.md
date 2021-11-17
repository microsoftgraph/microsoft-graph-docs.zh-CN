---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 949b75be6e15bce7114a3de3d5b46262ba908b6a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61029812"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewActivityBasedTimeoutPolicy()
requestBody.SetDefinition( []String {
    "definition-value",
}
displayName := "displayName-value"
requestBody.SetDisplayName(&displayName)
isOrganizationDefault := true
requestBody.SetIsOrganizationDefault(&isOrganizationDefault)
options := &msgraphsdk.ActivityBasedTimeoutPoliciesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Policies().ActivityBasedTimeoutPolicies().Post(options)


```