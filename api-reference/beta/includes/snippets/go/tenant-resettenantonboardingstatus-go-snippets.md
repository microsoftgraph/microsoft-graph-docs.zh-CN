---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3b84be0f169e7228183a95f720311f80f3251bc6
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412294"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

tenantId := "tenant-id"
result, err := graphClient.TenantRelationships().ManagedTenants().TenantsById(&tenantId).ResetTenantOnboardingStatus(tenant-id).Post(nil)


```