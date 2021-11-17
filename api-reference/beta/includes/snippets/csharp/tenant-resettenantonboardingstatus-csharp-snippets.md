---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: df4d9d584f27eab8ae4474d2520f192392134471992b600f7f2b5a94870c4856
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163396"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.TenantRelationships.ManagedTenants.Tenants["{managedTenants.tenant-id}"]
    .ResetTenantOnboardingStatus()
    .Request()
    .PostAsync();

```