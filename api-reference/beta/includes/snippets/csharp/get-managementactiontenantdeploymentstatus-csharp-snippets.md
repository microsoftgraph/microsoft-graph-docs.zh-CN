---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5faf799abf22b42952eb26deb62f665487156b8affc9734d2aed41e76ffa6b10
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278073"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var managementActionTenantDeploymentStatus = await graphClient.TenantRelationships.ManagedTenants.ManagementActionTenantDeploymentStatuses["{managedTenants.managementActionTenantDeploymentStatus-id}"]
    .Request()
    .GetAsync();

```