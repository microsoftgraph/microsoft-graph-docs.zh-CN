---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aac2cc6ae1894403bb87c01ac390898804def7e0
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441060"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tenantTag = await graphClient.TenantRelationships.ManagedTenants.TenantTags["{managedTenants.tenantTag-id}"]
    .Request()
    .GetAsync();

```