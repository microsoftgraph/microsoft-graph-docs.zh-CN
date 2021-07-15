---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 75cb8ea6f2b117462420e0f6b876f93ddebdf6aa
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442760"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tenantIds = new List<String>()
{
    "String"
};

await graphClient.TenantRelationships.ManagedTenants.TenantTags["{managedTenants.tenantTag-id}"]
    .UnassignTag(tenantIds)
    .Request()
    .PostAsync();

```