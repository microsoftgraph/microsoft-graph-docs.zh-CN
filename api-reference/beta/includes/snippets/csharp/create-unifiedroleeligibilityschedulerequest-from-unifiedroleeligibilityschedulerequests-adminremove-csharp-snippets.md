---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dbf37ccf2098867bf249a1cd95e7cb4bcf05a3bd
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58513982"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleEligibilityScheduleRequest = new UnifiedRoleEligibilityScheduleRequestObject
{
    Action = "AdminRemove",
    Justification = "Assign User Admin eligibility to IT Helpdesk (User) group",
    RoleDefinitionId = "fdd7a751-b60b-444a-984c-02652fe8fa1c",
    DirectoryScopeId = "/",
    PrincipalId = "07706ff1-46c7-4847-ae33-3003830675a1",
    ScheduleInfo = new RequestSchedule
    {
        StartDateTime = DateTimeOffset.Parse("2021-07-26T18:08:06.2081758Z"),
        Expiration = new ExpirationPattern
        {
            EndDateTime = DateTimeOffset.Parse("2022-06-30T00:00:00Z"),
            Type = ExpirationPatternType.AfterDateTime
        }
    }
};

await graphClient.RoleManagement.Directory.RoleEligibilityScheduleRequests
    .Request()
    .AddAsync(unifiedRoleEligibilityScheduleRequest);

```