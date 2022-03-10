---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c58d56260bed30aa8c2401d9e3ce3a5d0cb8f177
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411809"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

tenantId := "tenant-id"
result, err := graphClient.TenantRelationships().ManagedTenants().TenantsById(&tenantId).OffboardTenant(tenant-id).Post(nil)


```