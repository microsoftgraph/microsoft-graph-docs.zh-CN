---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e940786a3dda24ddd16ef0c69ba85312f73a6bb4
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61102287"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

tenantId := "tenant-id"
result, err := graphClient.TenantRelationships().ManagedTenants().TenantsById(&tenantId).ResetTenantOnboardingStatus().Post(options)


```