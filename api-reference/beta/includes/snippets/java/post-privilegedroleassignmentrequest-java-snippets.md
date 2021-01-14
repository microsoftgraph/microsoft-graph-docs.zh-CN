---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8a37c95e23afbdf9bef4e7898b1fa15c9f330999
ms.sourcegitcommit: dbbf77c732ae8d982e59865432b9b6147002a30a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/14/2021
ms.locfileid: "49866144"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrivilegedRoleAssignmentRequest privilegedRoleAssignmentRequest = new PrivilegedRoleAssignmentRequest();
privilegedRoleAssignmentRequest.duration = "2";
privilegedRoleAssignmentRequest.reason = "Activate the role for business purpose";
privilegedRoleAssignmentRequest.ticketNumber = "234";
privilegedRoleAssignmentRequest.ticketSystem = "system";
GovernanceSchedule schedule = new GovernanceSchedule();
schedule.startDateTime = CalendarSerializer.deserialize("2018-02-08T02:35:17.903Z");
privilegedRoleAssignmentRequest.schedule = schedule;
privilegedRoleAssignmentRequest.type = "UserAdd";
privilegedRoleAssignmentRequest.assignmentState = "Active";
privilegedRoleAssignmentRequest.roleId = "88d8e3e3-8f55-4a1e-953a-9b9898b8876b";

graphClient.privilegedRoleAssignmentRequests()
    .buildRequest()
    .post(privilegedRoleAssignmentRequest);

```