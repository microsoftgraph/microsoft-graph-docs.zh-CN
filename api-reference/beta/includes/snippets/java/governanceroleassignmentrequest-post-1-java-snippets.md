---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6727590ee7d82eb507f01e0069454de8c783fa66
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950748"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GovernanceRoleAssignmentRequest governanceRoleAssignmentRequest = new GovernanceRoleAssignmentRequest();
governanceRoleAssignmentRequest.roleDefinitionId = "ea48ad5e-e3b0-4d10-af54-39a45bbfe68d";
governanceRoleAssignmentRequest.resourceId = "e5e7d29d-5465-45ac-885f-4716a5ee74b5";
governanceRoleAssignmentRequest.subjectId = "918e54be-12c4-4f4c-a6d3-2ee0e3661c51";
governanceRoleAssignmentRequest.assignmentState = "Eligible";
governanceRoleAssignmentRequest.type = "AdminAdd";
governanceRoleAssignmentRequest.reason = "Assign an eligible role";
GovernanceSchedule schedule = new GovernanceSchedule();
schedule.startDateTime = CalendarSerializer.deserialize("2018-05-12T23:37:43.356Z");
schedule.endDateTime = CalendarSerializer.deserialize("2018-11-08T23:37:43.356Z");
schedule.type = "Once";
governanceRoleAssignmentRequest.schedule = schedule;

graphClient.privilegedAccess("azureResources").roleAssignmentRequests()
    .buildRequest()
    .post(governanceRoleAssignmentRequest);

```