---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f6b69be282291c2805561e9602b18fbd74618a6d
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089875"
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
options := &msgraphsdk.HomeRealmDiscoveryPoliciesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Policies().HomeRealmDiscoveryPolicies().Post(options)


```