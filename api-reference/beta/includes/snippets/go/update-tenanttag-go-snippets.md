---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 94c980489043cc1c6bc332d2d39d7da25bbcc1a3
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412755"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTenantTag()
displayName := "Onboarding"
requestBody.SetDisplayName(&displayName)
description := "Tenants that we are currently onboarding"
requestBody.SetDescription(&description)
options := &msgraphsdk.TenantTagRequestBuilderPatchOptions{
    Body: requestBody,
}
tenantTagId := "tenantTag-id"
result, err := graphClient.TenantRelationships().ManagedTenants().TenantTagsById(&tenantTagId).Patch(options)


```