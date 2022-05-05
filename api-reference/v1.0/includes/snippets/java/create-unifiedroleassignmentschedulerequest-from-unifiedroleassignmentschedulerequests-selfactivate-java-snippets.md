---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ff5dd3bf2eceadc97f530c0ad4e8955db085dd2
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65206768"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignmentScheduleRequest unifiedRoleAssignmentScheduleRequest = new UnifiedRoleAssignmentScheduleRequest();
unifiedRoleAssignmentScheduleRequest.action = UnifiedRoleScheduleRequestActions.SELF_ACTIVATE;
unifiedRoleAssignmentScheduleRequest.principalId = "071cc716-8147-4397-a5ba-b2105951cc0b";
unifiedRoleAssignmentScheduleRequest.roleDefinitionId = "8424c6f0-a189-499e-bbd0-26c1753c96d4";
unifiedRoleAssignmentScheduleRequest.directoryScopeId = "/";
unifiedRoleAssignmentScheduleRequest.justification = "I need access to the Attribute Administrator role to manage attributes to be assigned to restricted AUs";
RequestSchedule scheduleInfo = new RequestSchedule();
scheduleInfo.startDateTime = OffsetDateTimeSerializer.deserialize("2022-04-14T00:00:00Z");
ExpirationPattern expiration = new ExpirationPattern();
expiration.type = ExpirationPatternType.AFTER_DURATION;
expiration.duration = DatatypeFactory.newInstance().newDuration("PT5H");
scheduleInfo.expiration = expiration;
unifiedRoleAssignmentScheduleRequest.scheduleInfo = scheduleInfo;
TicketInfo ticketInfo = new TicketInfo();
ticketInfo.ticketNumber = "CONTOSO:Normal-67890";
ticketInfo.ticketSystem = "MS Project";
unifiedRoleAssignmentScheduleRequest.ticketInfo = ticketInfo;

graphClient.roleManagement().directory().roleAssignmentScheduleRequests()
    .buildRequest()
    .post(unifiedRoleAssignmentScheduleRequest);

```