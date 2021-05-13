---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 09650cf6573eb18442291fd15fb2dfeb3da1f0fa
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475493"
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

graphClient.roleManagement().directory().roleAssignmentScheduleRequests()
    .buildRequest()
    .post(unifiedRoleAssignmentScheduleRequest);

```