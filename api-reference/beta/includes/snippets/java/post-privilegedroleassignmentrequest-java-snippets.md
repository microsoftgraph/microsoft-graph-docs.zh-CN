---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6f4f0079fd9fcee79197c1d4e50608188c210e75
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875537"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrivilegedRoleAssignmentRequest privilegedRoleAssignmentRequest = new PrivilegedRoleAssignmentRequest();
privilegedRoleAssignmentRequest.duration = "2";
privilegedRoleAssignmentRequest.reason = "Activate the role for business purpose";
privilegedRoleAssignmentRequest.ticketNumber = "234";
privilegedRoleAssignmentRequest.ticketSystem = "system";
GovernanceSchedule schedule = new GovernanceSchedule();
schedule.startDateTime = "2018-02-08T02:35:17.903Z";
privilegedRoleAssignmentRequest.schedule = schedule;
privilegedRoleAssignmentRequest.evaluateOnly = false;
privilegedRoleAssignmentRequest.type = "UserAdd";
privilegedRoleAssignmentRequest.assignmentState = "Active";
privilegedRoleAssignmentRequest.roleId = "88d8e3e3-8f55-4a1e-953a-9b9898b8876b";

graphClient.privilegedRoleAssignmentRequests()
    .buildRequest()
    .post(privilegedRoleAssignmentRequest);

```