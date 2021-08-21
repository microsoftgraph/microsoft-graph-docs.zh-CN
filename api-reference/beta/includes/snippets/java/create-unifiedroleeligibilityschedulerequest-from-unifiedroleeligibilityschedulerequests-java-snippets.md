---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9abbde61df70457b881b8b43c921b7a08ce6a4a2d0a3bbe6f45f05dd4c3e371e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378375"
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

graphClient.roleManagement().directory().roleEligibilityScheduleRequests()
    .buildRequest()
    .post(unifiedRoleEligibilityScheduleRequest);

```