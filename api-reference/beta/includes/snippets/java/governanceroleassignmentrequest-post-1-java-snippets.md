---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4535cf1ec8be96980855755789dfca93b55862693cc0b956c2ff5e34fd621127
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105751"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GovernanceRoleAssignmentRequest governanceRoleAssignmentRequest = new GovernanceRoleAssignmentRequest();
governanceRoleAssignmentRequest.roleDefinitionId = "ea48ad5e-e3b0-4d10-af54-39a45bbfe68d";
governanceRoleAssignmentRequest.resourceId = "e5e7d29d-5465-45ac-885f-4716a5ee74b5";
governanceRoleAssignmentRequest.subjectId = "918e54be-12c4-4f4c-a6d3-2ee0e3661c51";
governanceRoleAssignmentRequest.assignmentState = "Eligible";
governanceRoleAssignmentRequest.type = "AdminAdd";
governanceRoleAssignmentRequest.reason = "Assign an eligible role";
GovernanceSchedule schedule = new GovernanceSchedule();
schedule.startDateTime = OffsetDateTimeSerializer.deserialize("2018-05-12T23:37:43.356Z");
schedule.endDateTime = OffsetDateTimeSerializer.deserialize("2018-11-08T23:37:43.356Z");
schedule.type = "Once";
governanceRoleAssignmentRequest.schedule = schedule;

graphClient.privilegedAccess("azureResources").roleAssignmentRequests()
    .buildRequest()
    .post(governanceRoleAssignmentRequest);

```