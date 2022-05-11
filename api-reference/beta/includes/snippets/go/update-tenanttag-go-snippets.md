---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3b936e8b6f651de1f99e07c2f37cf919fbd00982
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328233"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTenantTag()
displayName := "Onboarding"
requestBody.SetDisplayName(&displayName)
description := "Tenants that we are currently onboarding"
requestBody.SetDescription(&description)
tenantTagId := "tenantTag-id"
graphClient.TenantRelationships().ManagedTenants().TenantTagsById(&tenantTagId).Patch(requestBody)


```