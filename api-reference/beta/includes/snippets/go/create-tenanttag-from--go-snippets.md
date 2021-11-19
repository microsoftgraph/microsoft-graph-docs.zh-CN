---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a9523459909e86aa2d075129ca6442e75fa4fc3
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097053"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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