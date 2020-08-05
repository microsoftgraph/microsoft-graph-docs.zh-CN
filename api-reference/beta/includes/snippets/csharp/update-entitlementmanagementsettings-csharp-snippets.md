---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 749cc16323dc68a730def845185ec8eac037002d
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566859"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var entitlementManagementSettings = new EntitlementManagementSettings
{
    ExternalUserLifecycleAction = "None"
};

await graphClient.IdentityGovernance.EntitlementManagement.Settings
    .Request()
    .UpdateAsync(entitlementManagementSettings);

```