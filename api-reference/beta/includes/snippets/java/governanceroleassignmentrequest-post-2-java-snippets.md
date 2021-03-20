---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ccbbb91e18dd800d1e49d0101928b288426d4d8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950747"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GovernanceRoleAssignmentRequest governanceRoleAssignmentRequest = new GovernanceRoleAssignmentRequest();
governanceRoleAssignmentRequest.roleDefinitionId = "8b4d1d51-08e9-4254-b0a6-b16177aae376";
governanceRoleAssignmentRequest.resourceId = "e5e7d29d-5465-45ac-885f-4716a5ee74b5";
governanceRoleAssignmentRequest.subjectId = "918e54be-12c4-4f4c-a6d3-2ee0e3661c51";
governanceRoleAssignmentRequest.assignmentState = "Active";
governanceRoleAssignmentRequest.type = "UserAdd";
governanceRoleAssignmentRequest.reason = "Activate the owner role";
GovernanceSchedule schedule = new GovernanceSchedule();
schedule.type = "Once";
schedule.startDateTime = CalendarSerializer.deserialize("2018-05-12T23:28:43.537Z");
schedule.duration = DatatypeFactory.newInstance().newDuration("PT9H");
governanceRoleAssignmentRequest.schedule = schedule;
governanceRoleAssignmentRequest.linkedEligibleRoleAssignmentId = "e327f4be-42a0-47a2-8579-0a39b025b394";

graphClient.privilegedAccess("azureResources").roleAssignmentRequests()
    .buildRequest()
    .post(governanceRoleAssignmentRequest);

```