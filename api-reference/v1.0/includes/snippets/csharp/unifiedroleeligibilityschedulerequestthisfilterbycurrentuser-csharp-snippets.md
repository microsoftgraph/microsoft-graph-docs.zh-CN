---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ac786dcb27efc67b1d2f29256c18a39e023802e8
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204776"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var filterByCurrentUser = await graphClient.RoleManagement.Directory.RoleEligibilityScheduleRequests
    .FilterByCurrentUser(RoleEligibilityScheduleRequestFilterByCurrentUserOptions.Principal)
    .Request()
    .GetAsync();

```