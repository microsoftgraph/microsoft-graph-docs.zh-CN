---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 39c81506cea90a0a672729902438f22e7243d8e3
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210487"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GovernanceRoleAssignmentRequest governanceRoleAssignmentRequest = new GovernanceRoleAssignmentRequest();
governanceRoleAssignmentRequest.roleDefinitionId = "bc75b4e6-7403-4243-bf2f-d1f6990be122";
governanceRoleAssignmentRequest.resourceId = "fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735";
governanceRoleAssignmentRequest.subjectId = "918e54be-12c4-4f4c-a6d3-2ee0e3661c51";
governanceRoleAssignmentRequest.assignmentState = "Active";
governanceRoleAssignmentRequest.type = "UserRemove";
governanceRoleAssignmentRequest.reason = "Deactivate the role";
governanceRoleAssignmentRequest.linkedEligibleRoleAssignmentId = "cb8a533e-02d5-42ad-8499-916b1e4822ec";

graphClient.privilegedAccess("azureResources").roleAssignmentRequests()
    .buildRequest()
    .post(governanceRoleAssignmentRequest);

```