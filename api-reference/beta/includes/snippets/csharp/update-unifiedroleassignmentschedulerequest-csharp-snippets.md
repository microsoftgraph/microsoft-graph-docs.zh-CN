---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa92454335e44c0c11f5698cad4e3ecf8dc98c8e
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475459"
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

await graphClient.RoleManagement.Directory.RoleAssignmentScheduleRequests["{unifiedRoleAssignmentScheduleRequest-id}"]
    .Request()
    .UpdateAsync(unifiedRoleAssignmentScheduleRequest);

```