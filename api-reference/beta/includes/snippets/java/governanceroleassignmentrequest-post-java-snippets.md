---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8aecf30e80bf26707d101cacb32362ccfdd17157
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965459"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GovernanceRoleAssignmentRequest governanceRoleAssignmentRequest = new GovernanceRoleAssignmentRequest();
governanceRoleAssignmentRequest.roleDefinitionId = "0e88fd18-50f5-4ee1-9104-01c3ed910065";
governanceRoleAssignmentRequest.resourceId = "e5e7d29d-5465-45ac-885f-4716a5ee74b5";
governanceRoleAssignmentRequest.subjectId = "74765671-9ca4-40d7-9e36-2f4a570608a6";
governanceRoleAssignmentRequest.assignmentState = "Eligible";
governanceRoleAssignmentRequest.type = "AdminExtend";
governanceRoleAssignmentRequest.reason = "extend role assignment";
GovernanceSchedule schedule = new GovernanceSchedule();
schedule.type = "Once";
schedule.startDateTime = CalendarSerializer.deserialize("2018-05-12T23:53:55.327Z");
schedule.endDateTime = CalendarSerializer.deserialize("2018-08-10T23:53:55.327Z");
governanceRoleAssignmentRequest.schedule = schedule;

graphClient.privilegedAccess("azureResources").roleAssignmentRequests()
    .buildRequest()
    .post(governanceRoleAssignmentRequest);

```