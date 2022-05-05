---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dfe0b17e9f864cbb4b453a7d6066f57f5b0741c9
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65206769"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignmentScheduleRequest unifiedRoleAssignmentScheduleRequest = new UnifiedRoleAssignmentScheduleRequest();
unifiedRoleAssignmentScheduleRequest.action = UnifiedRoleScheduleRequestActions.ADMIN_ASSIGN;
unifiedRoleAssignmentScheduleRequest.justification = "Assign Groups Admin to IT Helpdesk group";
unifiedRoleAssignmentScheduleRequest.roleDefinitionId = "fdd7a751-b60b-444a-984c-02652fe8fa1c";
unifiedRoleAssignmentScheduleRequest.directoryScopeId = "/";
unifiedRoleAssignmentScheduleRequest.principalId = "071cc716-8147-4397-a5ba-b2105951cc0b";
RequestSchedule scheduleInfo = new RequestSchedule();
scheduleInfo.startDateTime = OffsetDateTimeSerializer.deserialize("2022-04-10T00:00:00Z");
ExpirationPattern expiration = new ExpirationPattern();
expiration.type = ExpirationPatternType.NO_EXPIRATION;
scheduleInfo.expiration = expiration;
unifiedRoleAssignmentScheduleRequest.scheduleInfo = scheduleInfo;

graphClient.roleManagement().directory().roleAssignmentScheduleRequests()
    .buildRequest()
    .post(unifiedRoleAssignmentScheduleRequest);

```