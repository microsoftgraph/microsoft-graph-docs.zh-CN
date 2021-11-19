---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b16b46b34d1ec00299926e9ca9d52969514ce575
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091635"
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
graphClient.TenantRelationships().ManagedTenants().TenantTagsById(&tenantTagId).Patch(options)


```