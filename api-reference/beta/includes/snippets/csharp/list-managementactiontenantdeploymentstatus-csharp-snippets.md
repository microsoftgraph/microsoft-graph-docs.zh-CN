---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3e2583f5fc310dba3f3f2dc2f9cb809d71afcd53e642606c6603f0d923b7e55a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106318"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var managementActionTenantDeploymentStatuses = await graphClient.TenantRelationships.ManagedTenants.ManagementActionTenantDeploymentStatuses
    .Request()
    .GetAsync();

```