---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b5602ef8006751b477b51285737b115fadb3b99b
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58513525"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleAssignmentScheduleRequest = new UnifiedRoleAssignmentScheduleRequestObject
{
    Action = "AdminAssign",
    Justification = "Assign User Admin to IT Helpdesk (User) group",
    RoleDefinitionId = "fdd7a751-b60b-444a-984c-02652fe8fa1c",
    DirectoryScopeId = "/",
    PrincipalId = "07706ff1-46c7-4847-ae33-3003830675a1",
    ScheduleInfo = new RequestSchedule
    {
        StartDateTime = DateTimeOffset.Parse("2021-07-01T00:00:00Z"),
        Expiration = new ExpirationPattern
        {
            Type = ExpirationPatternType.NoExpiration
        }
    }
};

await graphClient.RoleManagement.Directory.RoleAssignmentScheduleRequests
    .Request()
    .AddAsync(unifiedRoleAssignmentScheduleRequest);

```