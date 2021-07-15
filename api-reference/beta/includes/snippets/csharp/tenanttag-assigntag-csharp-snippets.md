---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 57448d1ca13ed6bc184489bb924dcb737e2c691e
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441746"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tenantIds = new List<String>()
{
    "String"
};

await graphClient.TenantRelationships.ManagedTenants.TenantTags["{managedTenants.tenantTag-id}"]
    .AssignTag(tenantIds)
    .Request()
    .PostAsync();

```