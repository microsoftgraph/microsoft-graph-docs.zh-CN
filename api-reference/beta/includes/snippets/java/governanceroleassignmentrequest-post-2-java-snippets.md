---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 497c5dd7ee3d5eccc0df328aed0193c79e73b7e2
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209291"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GovernanceRoleAssignmentRequest governanceRoleAssignmentRequest = new GovernanceRoleAssignmentRequest();
governanceRoleAssignmentRequest.roleDefinitionId = "8b4d1d51-08e9-4254-b0a6-b16177aae376";
governanceRoleAssignmentRequest.resourceId = "e5e7d29d-5465-45ac-885f-4716a5ee74b5";
governanceRoleAssignmentRequest.subjectId = "918e54be-12c4-4f4c-a6d3-2ee0e3661c51";
governanceRoleAssignmentRequest.assignmentState = "Active";
governanceRoleAssignmentRequest.type = "UserAdd";
governanceRoleAssignmentRequest.reason = "Activate the owner role";
GovernanceSchedule schedule = new GovernanceSchedule();
schedule.type = "Once";
schedule.startDateTime = OffsetDateTimeSerializer.deserialize("2018-05-12T23:28:43.537Z");
schedule.duration = DatatypeFactory.newInstance().newDuration("PT9H");
governanceRoleAssignmentRequest.schedule = schedule;
governanceRoleAssignmentRequest.linkedEligibleRoleAssignmentId = "e327f4be-42a0-47a2-8579-0a39b025b394";

graphClient.privilegedAccess("azureResources").roleAssignmentRequests()
    .buildRequest()
    .post(governanceRoleAssignmentRequest);

```