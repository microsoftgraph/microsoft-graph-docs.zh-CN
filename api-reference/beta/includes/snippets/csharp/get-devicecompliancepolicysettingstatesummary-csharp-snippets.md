---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 85b0f740e202446e5499d82c3728996df079790e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62131014"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var deviceCompliancePolicySettingStateSummary = await graphClient.TenantRelationships.ManagedTenants.DeviceCompliancePolicySettingStateSummaries["{managedTenants.deviceCompliancePolicySettingStateSummary-id}"]
    .Request()
    .GetAsync();

```