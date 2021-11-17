---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 878e293396b737e2ae51af3f668020c3fe93521f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61034208"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewTenantTag()
displayName := "Support"
requestBody.SetDisplayName(&displayName)
description := "Tenants that have purchased extended support"
requestBody.SetDescription(&description)
options := &msgraphsdk.TenantTagsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.TenantRelationships().ManagedTenants().TenantTags().Post(options)


```