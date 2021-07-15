---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: be4c8bc29e74f999185b83641701cc0575166ea8
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442119"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tenantId = "String";

var tenantGroupId = "String";

var managementTemplateId = "String";

await graphClient.TenantRelationships.ManagedTenants.ManagementActions["{managedTenants.managementAction-id}"]
    .Apply(tenantId,tenantGroupId,managementTemplateId)
    .Request()
    .PostAsync();

```