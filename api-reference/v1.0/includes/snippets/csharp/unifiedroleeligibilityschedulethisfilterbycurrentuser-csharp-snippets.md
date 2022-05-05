---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c7d5f17aa7e805e4a8760007e4d117cf825b5e9d
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65205029"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var filterByCurrentUser = await graphClient.RoleManagement.Directory.RoleEligibilitySchedules
    .FilterByCurrentUser(RoleEligibilityScheduleFilterByCurrentUserOptions.Principal)
    .Request()
    .GetAsync();

```