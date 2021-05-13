---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ed2cf694f45218bb864cdb6dfb95f53d5111336d
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475460"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignmentScheduleRequest unifiedRoleAssignmentScheduleRequest = new UnifiedRoleAssignmentScheduleRequest();
unifiedRoleAssignmentScheduleRequest.action = "String";
unifiedRoleAssignmentScheduleRequest.principalId = "String";
unifiedRoleAssignmentScheduleRequest.roleDefinitionId = "String";
unifiedRoleAssignmentScheduleRequest.directoryScopeId = "String";
unifiedRoleAssignmentScheduleRequest.appScopeId = "String";
unifiedRoleAssignmentScheduleRequest.isValidationOnly = false;
unifiedRoleAssignmentScheduleRequest.targetScheduleId = "String";
unifiedRoleAssignmentScheduleRequest.justification = "String";
RequestSchedule scheduleInfo = new RequestSchedule();
unifiedRoleAssignmentScheduleRequest.scheduleInfo = scheduleInfo;
TicketInfo ticketInfo = new TicketInfo();
unifiedRoleAssignmentScheduleRequest.ticketInfo = ticketInfo;

graphClient.roleManagement().directory().roleAssignmentScheduleRequests("{unifiedRoleAssignmentScheduleRequestsId}")
    .buildRequest()
    .patch(unifiedRoleAssignmentScheduleRequest);

```