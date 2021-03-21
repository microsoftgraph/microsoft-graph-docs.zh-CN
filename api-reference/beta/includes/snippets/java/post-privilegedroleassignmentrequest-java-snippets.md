---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ad9b7d8e36300cc23d88f4936a95dc6a4128aab
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976536"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrivilegedRoleAssignmentRequest privilegedRoleAssignmentRequest = new PrivilegedRoleAssignmentRequest();
privilegedRoleAssignmentRequest.duration = "2";
privilegedRoleAssignmentRequest.reason = "Activate the role for business purpose";
privilegedRoleAssignmentRequest.ticketNumber = "234";
privilegedRoleAssignmentRequest.ticketSystem = "system";
GovernanceSchedule schedule = new GovernanceSchedule();
schedule.startDateTime = OffsetDateTimeSerializer.deserialize("2018-02-08T02:35:17.903Z");
privilegedRoleAssignmentRequest.schedule = schedule;
privilegedRoleAssignmentRequest.type = "UserAdd";
privilegedRoleAssignmentRequest.assignmentState = "Active";
privilegedRoleAssignmentRequest.roleId = "88d8e3e3-8f55-4a1e-953a-9b9898b8876b";

graphClient.privilegedRoleAssignmentRequests()
    .buildRequest()
    .post(privilegedRoleAssignmentRequest);

```