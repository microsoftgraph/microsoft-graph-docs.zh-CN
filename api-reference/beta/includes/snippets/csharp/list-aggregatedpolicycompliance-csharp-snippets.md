---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a2b7b834e0b566f0aaabeb721376f4a09586b9e435353389adb3a35ccb7d16f6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221323"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var aggregatedPolicyCompliances = await graphClient.TenantRelationships.ManagedTenants.AggregatedPolicyCompliances
    .Request()
    .GetAsync();

```