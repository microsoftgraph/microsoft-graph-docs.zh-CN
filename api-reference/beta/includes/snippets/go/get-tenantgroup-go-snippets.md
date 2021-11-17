---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a58c0f7183ae0d44be75d9c8ee7a0263f4ca2df
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61019801"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

tenantGroupId := "tenantGroup-id"
result, err := graphClient.TenantRelationships().ManagedTenants().TenantGroupsById(&tenantGroupId).Get(options)


```