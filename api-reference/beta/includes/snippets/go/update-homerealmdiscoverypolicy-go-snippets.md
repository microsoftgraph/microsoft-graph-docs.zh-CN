---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f4a2e6fd0ae0662c3368e47c94f72709caa4cde0
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60986228"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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