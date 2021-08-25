---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2b4999190ce8baa107334d9593832e6d79ea5b3e
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58513522"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignmentScheduleRequest unifiedRoleAssignmentScheduleRequest = new UnifiedRoleAssignmentScheduleRequest();
unifiedRoleAssignmentScheduleRequest.action = "AdminAssign";
unifiedRoleAssignmentScheduleRequest.justification = "Assign User Admin to IT Helpdesk (User) group";
unifiedRoleAssignmentScheduleRequest.roleDefinitionId = "fdd7a751-b60b-444a-984c-02652fe8fa1c";
unifiedRoleAssignmentScheduleRequest.directoryScopeId = "/";
unifiedRoleAssignmentScheduleRequest.principalId = "07706ff1-46c7-4847-ae33-3003830675a1";
RequestSchedule scheduleInfo = new RequestSchedule();
scheduleInfo.startDateTime = OffsetDateTimeSerializer.deserialize("2021-07-01T00:00:00Z");
ExpirationPattern expiration = new ExpirationPattern();
expiration.type = ExpirationPatternType.NO_EXPIRATION;
scheduleInfo.expiration = expiration;
unifiedRoleAssignmentScheduleRequest.scheduleInfo = scheduleInfo;

graphClient.roleManagement().directory().roleAssignmentScheduleRequests()
    .buildRequest()
    .post(unifiedRoleAssignmentScheduleRequest);

```