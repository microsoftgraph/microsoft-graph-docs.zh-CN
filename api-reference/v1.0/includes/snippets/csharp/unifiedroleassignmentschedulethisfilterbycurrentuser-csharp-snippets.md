---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d5418270273f8a24d434a23288065c91bcd35502
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65205345"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var filterByCurrentUser = await graphClient.RoleManagement.Directory.RoleAssignmentSchedules
    .FilterByCurrentUser(RoleAssignmentScheduleFilterByCurrentUserOptions.Principal)
    .Request()
    .GetAsync();

```