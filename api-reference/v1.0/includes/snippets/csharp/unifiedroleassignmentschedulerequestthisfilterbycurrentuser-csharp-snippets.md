---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eec48b9ead65f7c7492a280691ad64d843534ef0
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65205147"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var filterByCurrentUser = await graphClient.RoleManagement.Directory.RoleAssignmentScheduleRequests
    .FilterByCurrentUser(RoleAssignmentScheduleRequestFilterByCurrentUserOptions.Principal)
    .Request()
    .GetAsync();

```