---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 092e98e183791cc83aae09effc5f40766fb2c59b
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51211006"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GovernanceRoleAssignmentRequest governanceRoleAssignmentRequest = new GovernanceRoleAssignmentRequest();
governanceRoleAssignmentRequest.roleDefinitionId = "70521f3e-3b95-4e51-b4d2-a2f485b02103";
governanceRoleAssignmentRequest.resourceId = "e5e7d29d-5465-45ac-885f-4716a5ee74b5";
governanceRoleAssignmentRequest.subjectId = "1566d11d-d2b6-444a-a8de-28698682c445";
governanceRoleAssignmentRequest.assignmentState = "Eligible";
governanceRoleAssignmentRequest.type = "AdminUpdate";
GovernanceSchedule schedule = new GovernanceSchedule();
schedule.type = "Once";
schedule.startDateTime = OffsetDateTimeSerializer.deserialize("2018-03-08T05:42:45.317Z");
schedule.endDateTime = OffsetDateTimeSerializer.deserialize("2018-06-05T05:42:31Z");
governanceRoleAssignmentRequest.schedule = schedule;

graphClient.privilegedAccess("azureResources").roleAssignmentRequests()
    .buildRequest()
    .post(governanceRoleAssignmentRequest);

```