---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 85f628302761d0089a63f9b8fb50d15eba109cfb
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412584"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTenantIdRequestBody()
tenantId := "String"
requestBody.SetTenantId(&tenantId)
options := &msgraphsdk.TenantSearchRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.TenantRelationships().ManagedTenants().TenantGroups().TenantSearch().Post(options)


```