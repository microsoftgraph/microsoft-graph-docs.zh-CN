---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3023b55e92074833b0373f5e7b0444fc53aee184
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204927"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var filterByCurrentUser = await graphClient.RoleManagement.Directory.RoleEligibilityScheduleInstances
    .FilterByCurrentUser(RoleEligibilityScheduleInstanceFilterByCurrentUserOptions.Principal)
    .Request()
    .GetAsync();

```