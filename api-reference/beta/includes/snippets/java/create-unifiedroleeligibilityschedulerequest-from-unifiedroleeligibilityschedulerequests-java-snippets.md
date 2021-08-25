---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 57250673b281646f4dcb4c0643cca09c4cb55219
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58513953"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleEligibilityScheduleRequest unifiedRoleEligibilityScheduleRequest = new UnifiedRoleEligibilityScheduleRequest();
unifiedRoleEligibilityScheduleRequest.action = "AdminAssign";
unifiedRoleEligibilityScheduleRequest.justification = "Assign User Admin eligibility to IT Helpdesk (User) group";
unifiedRoleEligibilityScheduleRequest.roleDefinitionId = "fdd7a751-b60b-444a-984c-02652fe8fa1c";
unifiedRoleEligibilityScheduleRequest.directoryScopeId = "/";
unifiedRoleEligibilityScheduleRequest.principalId = "07706ff1-46c7-4847-ae33-3003830675a1";
RequestSchedule scheduleInfo = new RequestSchedule();
scheduleInfo.startDateTime = OffsetDateTimeSerializer.deserialize("2021-07-01T00:00:00Z");
ExpirationPattern expiration = new ExpirationPattern();
expiration.endDateTime = OffsetDateTimeSerializer.deserialize("2022-06-30T00:00:00Z");
expiration.type = ExpirationPatternType.AFTER_DATE_TIME;
scheduleInfo.expiration = expiration;
unifiedRoleEligibilityScheduleRequest.scheduleInfo = scheduleInfo;

graphClient.roleManagement().directory().roleEligibilityScheduleRequests()
    .buildRequest()
    .post(unifiedRoleEligibilityScheduleRequest);

```