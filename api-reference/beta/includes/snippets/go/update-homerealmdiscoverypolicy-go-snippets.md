---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 92afe072d65e5b71cc15ad09b1882d2e134ad70c
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61093632"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewHomeRealmDiscoveryPolicy()
requestBody.SetDefinition( []String {
    "definition-value",
}
displayName := "displayName-value"
requestBody.SetDisplayName(&displayName)
isOrganizationDefault := true
requestBody.SetIsOrganizationDefault(&isOrganizationDefault)
options := &msgraphsdk.HomeRealmDiscoveryPolicyRequestBuilderPatchOptions{
    Body: requestBody,
}
homeRealmDiscoveryPolicyId := "homeRealmDiscoveryPolicy-id"
graphClient.Policies().HomeRealmDiscoveryPoliciesById(&homeRealmDiscoveryPolicyId).Patch(options)


```