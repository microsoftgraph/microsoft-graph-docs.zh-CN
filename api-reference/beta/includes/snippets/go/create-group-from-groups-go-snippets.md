---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a6b0a3f99aca3f58389c38e7c32873be6c78a02
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220277"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/odata/groups('1a9db3ab-0acf-4808-99ae-e8ed581cb2e0')",
}
options := &msgraphsdk.GroupRequestBuilderPostOptions{
    Body: requestBody,
}
mobilityManagementPolicyId := "mobilityManagementPolicy-id"
groupId := "group-id"
graphClient.Policies().MobileAppManagementPoliciesById(&mobilityManagementPolicyId).IncludedGroupsById(&groupId).Post(options)


```