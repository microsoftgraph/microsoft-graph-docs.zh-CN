---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8ca394fabbed679a90ae1d5cf604f1300390441e
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59507870"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var includedGroups = await graphClient.Policies.MobileAppManagementPolicies["{mobilityManagementPolicy-id}"].IncludedGroups
    .Request()
    .GetAsync();

```