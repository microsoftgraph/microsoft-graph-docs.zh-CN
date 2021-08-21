---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 46f9e66f3ea94991d3b91219dd92fdad9c09b994c2a47f3d9087ad0f62deb2b5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903604"
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