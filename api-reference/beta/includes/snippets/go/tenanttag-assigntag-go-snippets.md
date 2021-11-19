---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 044656a07719b862936cbaf99851a7c54e5e8a39
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61088791"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetTenantIds( []String {
    "String",
}
options := &msgraphsdk.AssignTagRequestBuilderPostOptions{
    Body: requestBody,
}
tenantTagId := "tenantTag-id"
result, err := graphClient.TenantRelationships().ManagedTenants().TenantTagsById(&tenantTagId).AssignTag().Post(options)


```