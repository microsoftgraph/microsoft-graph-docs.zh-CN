---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a0f10b42937fc502c7bb40014a01b20fd601be121eb5f934c45e4a84d51cd87
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163972"
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