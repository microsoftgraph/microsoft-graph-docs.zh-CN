---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 163783d2735c55105ca2323b074eccc86fe09930
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441614"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var managedDeviceComplianceTrend = await graphClient.TenantRelationships.ManagedTenants.ManagedDeviceComplianceTrends["{managedTenants.managedDeviceComplianceTrend-id}"]
    .Request()
    .GetAsync();

```