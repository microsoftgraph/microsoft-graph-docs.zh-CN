---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: abe70a024375497478784bbef23a2c68f67eb5c8
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48976189"
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
privilegedRoleAssignmentRequest.evaluateOnly = false;
privilegedRoleAssignmentRequest.type = "UserAdd";
privilegedRoleAssignmentRequest.assignmentState = "Active";
privilegedRoleAssignmentRequest.roleId = "88d8e3e3-8f55-4a1e-953a-9b9898b8876b";

graphClient.privilegedRoleAssignmentRequests()
    .buildRequest()
    .post(privilegedRoleAssignmentRequest);

```