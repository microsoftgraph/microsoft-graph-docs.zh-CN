---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3df0c8aba82cfb6be2d6a7ddf492149bf2adcf7a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61014607"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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