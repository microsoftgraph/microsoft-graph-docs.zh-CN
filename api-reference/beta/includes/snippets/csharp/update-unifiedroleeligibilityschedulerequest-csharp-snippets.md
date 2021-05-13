---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: da01fd8ab2a125a9bcc43074adb3af338c860827
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474380"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleEligibilityScheduleRequest = new UnifiedRoleEligibilityScheduleRequestObject
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

await graphClient.RoleManagement.Directory.RoleEligibilityScheduleRequests["{unifiedRoleEligibilityScheduleRequest-id}"]
    .Request()
    .UpdateAsync(unifiedRoleEligibilityScheduleRequest);

```