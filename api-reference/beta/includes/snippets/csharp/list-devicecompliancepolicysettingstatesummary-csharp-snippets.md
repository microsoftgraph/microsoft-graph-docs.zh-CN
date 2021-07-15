---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 426b461468c5bcf6b1b44d609c7db968d1da485c
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441999"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var deviceCompliancePolicySettingStateSummary = await graphClient.TenantRelationships.ManagedTenants.DeviceCompliancePolicySettingStateSummary
    .Request()
    .GetAsync();

```