---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2964888eb5011f3f7d03459ed3546eff0f5b4a9ccf273d9c11b091e4fc3516b5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278075"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var managementTemplates = await graphClient.TenantRelationships.ManagedTenants.ManagementTemplates
    .Request()
    .GetAsync();

```