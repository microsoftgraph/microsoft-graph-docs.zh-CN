---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 620f8070f988b8238f4e5bdf7fede0d03e101770
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61085686"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewActivityBasedTimeoutPolicy()
requestBody.SetDefinition( []String {
    "definition-value",
}
displayName := "displayName-value"
requestBody.SetDisplayName(&displayName)
isOrganizationDefault := true
requestBody.SetIsOrganizationDefault(&isOrganizationDefault)
options := &msgraphsdk.ActivityBasedTimeoutPolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
activityBasedTimeoutPolicyId := "activityBasedTimeoutPolicy-id"
graphClient.Policies().ActivityBasedTimeoutPoliciesById(&activityBasedTimeoutPolicyId).Patch(options)


```