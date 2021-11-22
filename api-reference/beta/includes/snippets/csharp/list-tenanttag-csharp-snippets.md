---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 890e71ad8a8f13c8fb0149235e4ba5830c0ce6969eb9dba39ffcd909ca79eaf7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220875"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tenantTags = await graphClient.TenantRelationships.ManagedTenants.TenantTags
    .Request()
    .GetAsync();

```