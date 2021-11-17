---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 32ad0871b90b13bd17b9dffe239935d3b2b5ce6a35972ff102e2c6845335cceb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218488"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tenantTag = await graphClient.TenantRelationships.ManagedTenants.TenantTags["{managedTenants.tenantTag-id}"]
    .Request()
    .GetAsync();

```