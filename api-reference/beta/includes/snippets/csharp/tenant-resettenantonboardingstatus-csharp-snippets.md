---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d0e62fe6926ac02e7431d7cdab8e942d99553f0
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440404"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.TenantRelationships.ManagedTenants.Tenants["{managedTenants.tenant-id}"]
    .ResetTenantOnboardingStatus()
    .Request()
    .PostAsync();

```