---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7bfb9d145adbb92a3ffa4191a615df32d7c66904
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474381"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleEligibilityScheduleRequest unifiedRoleEligibilityScheduleRequest = new UnifiedRoleEligibilityScheduleRequest();
unifiedRoleEligibilityScheduleRequest.action = "String";
unifiedRoleEligibilityScheduleRequest.principalId = "String";
unifiedRoleEligibilityScheduleRequest.roleDefinitionId = "String";
unifiedRoleEligibilityScheduleRequest.directoryScopeId = "String";
unifiedRoleEligibilityScheduleRequest.appScopeId = "String";
unifiedRoleEligibilityScheduleRequest.isValidationOnly = false;
unifiedRoleEligibilityScheduleRequest.targetScheduleId = "String";
unifiedRoleEligibilityScheduleRequest.justification = "String";
RequestSchedule scheduleInfo = new RequestSchedule();
unifiedRoleEligibilityScheduleRequest.scheduleInfo = scheduleInfo;
TicketInfo ticketInfo = new TicketInfo();
unifiedRoleEligibilityScheduleRequest.ticketInfo = ticketInfo;

graphClient.roleManagement().directory().roleEligibilityScheduleRequests("{unifiedRoleEligibilityScheduleRequestsId}")
    .buildRequest()
    .patch(unifiedRoleEligibilityScheduleRequest);

```