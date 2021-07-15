---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ff361b6d422b2e6cf888c5545dcb1877b47ba3b
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441522"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var aggregatedPolicyCompliances = await graphClient.TenantRelationships.ManagedTenants.AggregatedPolicyCompliances
    .Request()
    .GetAsync();

```