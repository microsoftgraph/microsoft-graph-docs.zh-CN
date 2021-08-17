---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 908d1a0c81858622054aa390d78a7d23e04bc045
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58262590"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies.MobileDeviceManagementPolicies["{mobilityManagementPolicy-id}"].IncludedGroups["{group-id}"].Reference
    .Request()
    .DeleteAsync();

```