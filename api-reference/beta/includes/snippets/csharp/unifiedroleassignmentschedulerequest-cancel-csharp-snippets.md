---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 668470afec1ed0a9fb7b7e5b2eeaf048e8406085
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475110"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.RoleManagement.Directory.RoleAssignmentScheduleRequests["{unifiedRoleAssignmentScheduleRequest-id}"]
    .Cancel()
    .Request()
    .PostAsync();

```