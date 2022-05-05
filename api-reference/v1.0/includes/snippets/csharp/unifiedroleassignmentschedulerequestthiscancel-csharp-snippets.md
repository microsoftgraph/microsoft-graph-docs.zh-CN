---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 668470afec1ed0a9fb7b7e5b2eeaf048e8406085
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65205185"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.RoleManagement.Directory.RoleAssignmentScheduleRequests["{unifiedRoleAssignmentScheduleRequest-id}"]
    .Cancel()
    .Request()
    .PostAsync();

```