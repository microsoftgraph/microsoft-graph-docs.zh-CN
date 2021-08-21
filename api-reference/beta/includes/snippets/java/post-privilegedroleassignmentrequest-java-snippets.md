---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 32459ed0282f37e258a05ff795c292dc7b2e8d224904b6166c000c89dca02a1f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106873"
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