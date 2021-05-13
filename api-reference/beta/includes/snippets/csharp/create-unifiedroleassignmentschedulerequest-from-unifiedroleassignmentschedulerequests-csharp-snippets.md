---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec4df566ffbf0fdef51a4994ea6b00da600fc675
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475510"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleAssignmentScheduleRequest = new UnifiedRoleAssignmentScheduleRequestObject
{
    Action = "String",
    PrincipalId = "String",
    RoleDefinitionId = "String",
    DirectoryScopeId = "String",
    AppScopeId = "String",
    IsValidationOnly = false,
    TargetScheduleId = "String",
    Justification = "String",
    ScheduleInfo = new RequestSchedule
    {
    },
    TicketInfo = new TicketInfo
    {
    }
};

await graphClient.RoleManagement.Directory.RoleAssignmentScheduleRequests
    .Request()
    .AddAsync(unifiedRoleAssignmentScheduleRequest);

```