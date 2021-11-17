---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eaec106894474e929474a558a4cf7ffdac43373f4fb8098e679fe46466a71834
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161210"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tenantsDetailedInformation = await graphClient.TenantRelationships.ManagedTenants.TenantsDetailedInformation
    .Request()
    .GetAsync();

```