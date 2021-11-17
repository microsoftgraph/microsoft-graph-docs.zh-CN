---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 96eb8c00e7382c0b543cd7897988c5f8fc6efac9
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61022076"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

tenantDetailedInformationId := "tenantDetailedInformation-id"
result, err := graphClient.TenantRelationships().ManagedTenants().TenantsDetailedInformationById(&tenantDetailedInformationId).Get(options)


```