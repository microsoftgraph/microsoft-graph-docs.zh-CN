---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b9cc15108294a20cc2f267ff2aa032f372e987e4
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65205291"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var filterByCurrentUser = await graphClient.RoleManagement.Directory.RoleAssignmentScheduleInstances
    .FilterByCurrentUser(RoleAssignmentScheduleInstanceFilterByCurrentUserOptions.Principal)
    .Request()
    .GetAsync();

```