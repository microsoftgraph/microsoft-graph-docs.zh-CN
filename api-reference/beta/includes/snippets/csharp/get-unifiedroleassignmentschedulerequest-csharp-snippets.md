---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0759953567e52f5400ef2bd75b8f48bca97eedd836aff806f8e67203e1ae36ab
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158439"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleAssignmentScheduleRequest = await graphClient.RoleManagement.Directory.RoleAssignmentScheduleRequests["{unifiedRoleAssignmentScheduleRequest-id}"]
    .Request()
    .GetAsync();

```