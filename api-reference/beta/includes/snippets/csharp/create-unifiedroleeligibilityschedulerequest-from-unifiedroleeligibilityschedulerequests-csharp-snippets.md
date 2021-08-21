---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c3c36de606b36f44e807f4c35b1e8c87d84322c0a97ff408338f77bdc1612da9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333687"
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

await graphClient.RoleManagement.Directory.RoleEligibilityScheduleRequests
    .Request()
    .AddAsync(unifiedRoleEligibilityScheduleRequest);

```