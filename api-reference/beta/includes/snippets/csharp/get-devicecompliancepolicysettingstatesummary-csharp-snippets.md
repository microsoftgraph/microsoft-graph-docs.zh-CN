---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1a78c3c6fa58b500bbf0767a8c0cd598733ef59d
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439969"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var response = await graphClient.TenantRelationships.ManagedTenants.DeviceCompliancePolicySettingStateSummarys["{UNKNOWN-id}"]
    .Request()
    .GetAsync();

```